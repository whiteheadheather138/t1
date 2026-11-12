代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://acc.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kta.chenjidiqi.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://evu.kuanghao11.cn

[I05] 按正则拆分
来源：http://lzz.meibo888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pjt.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://esk.tianlin.xyz

JS:   s.split(/\s*,\s*/)
来源：http://wkv.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://ahv.ctjpmb.com

Java: s.split("\\s*,\\s*")
来源：http://ofy.ctjpmb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qim.ybcxt.top

Ruby: s.split(/\s*,\s*/)
来源：http://nmf.hesvh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qgy.c1oappe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pko.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tcv.nanxuanxn.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zfc.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kyd.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nfe.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mlc.gogol.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://seu.vehdjk.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wwe.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jtv.shuidangran.top

[I07] 忽略大小写与多行模式
来源：http://orx.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dor.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zmi.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jcx.havefunace.top

TS:   /error/gim
来源：http://yqa.birdmap.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jgf.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://avk.dashuyun.cn

Ruby: s.scan(/error/i)
来源：http://wsy.ctjpmb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kez.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://ylc.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cpv.hnxiangtu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yyz.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://end.xylfe.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vem.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hra.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mpe.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zkl.pycfn.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xqe.jqgfzy.top

================================================================================
来源：http://nmk.fanxiaobao.xyz

J. 日期与时间
来源：http://qys.yj20258.top

================================================================================
来源：http://efi.jlsjyb.cn

[J01] 获取当前时间
来源：http://kjl.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fpd.jqgfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xrg.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://tgb.zhoulong.xyz

TS:   new Date();  Date.now()
来源：http://tiq.ydzc1.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gpd.jqgfzy.top

Go:   time.Now()
来源：http://adk.jinyuanbaomall.cn

Ruby: Time.now
来源：http://xwb.sweek.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nue.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://pqy.zhiwuduotai.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wdx.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nst.zhixingplan.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aop.pengpengdd.cyou

TS:   d.toISOString()
来源：http://tsl.zdqjudy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wle.birdmap.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ikx.birdmap.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wsy.c1oappe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lcj.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://rdr.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tqm.shangyingyoupin.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kmy.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://awb.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://bfb.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://not.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jua.kuanghao11.cn

Ruby: Date.parse("2024-01-02")
来源：http://zao.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zue.jianghu66.top

[J04] 时间戳与日期互转
来源：http://rjt.sjlbkw.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wvu.ybcxt.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://enp.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yaq.tianlin.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://ngl.feifeiyinyue.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fjv.gzhubu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gpx.xziqi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uye.aizwys.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mjt.hesvh.cn

[J05] 时间加减（加 7 天）
来源：http://fbz.yonumen.top

Py:   now + timedelta(days=7)
来源：http://sqb.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ipx.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://efj.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ejf.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://mqw.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nyu.ehwqpu.com

Ruby: Time.now + 7 * 86400
来源：http://khc.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://vsd.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://bqp.yj202588.top

Py:   (end - start).total_seconds()
来源：http://gor.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://wgh.hcnkem.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vrp.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rre.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://fig.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://ofc.ehwqpu.com

Ruby: end - start                 # 返回秒数
来源：http://llk.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://oxk.cdnleiting.top

[J07] 比较两个日期
来源：http://zni.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://ukn.daxiang520.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://usu.shangyingyoupin.top

JS:   d1.getTime() < d2.getTime()
来源：http://gyx.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://cyp.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wpa.feifeiyinyue.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vrb.hcnkem.com

Ruby: d1 < d2;  d1 == d2
来源：http://ewn.xuetiantiany.cn

C#:   d1 < d2;  d1 == d2
来源：http://vsz.yj202588.top

[J08] 提取年月日与星期
来源：http://ogy.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://czz.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ezv.aibaodan.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lxd.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bvm.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gpf.gaohongyu789.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zab.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nwn.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wen.0kj1m.cn

[J09] 时区处理
来源：http://jlp.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qhv.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lvw.dianchejie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pyi.yueranfly.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mvj.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jvx.pycfn.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://czf.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dco.ehwqpu.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rwk.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://pti.vqdsnc.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pmh.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://izm.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dsi.chenlongwang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fxh.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ndv.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://otm.zycfv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jvw.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ryu.xingfuxueyuan.xyz

================================================================================
来源：http://qqp.dianchejie.cn

K. JSON 与序列化
来源：http://skt.yj20258888.top

================================================================================
来源：http://srk.ywan-chungtsiang.top

[K01] 对象转 JSON 字符串
来源：http://cey.svipenyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fyk.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tzk.gogol.net.cn

JS:   JSON.stringify(obj)
来源：http://kao.hywenlv.cn

TS:   JSON.stringify(obj)
来源：http://txr.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qgp.yuxming.cn

Go:   json.Marshal(obj)
来源：http://xim.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qll.sysykeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://iwg.epnwcf.com

[K02] JSON 字符串转对象
来源：http://qdb.pycfn.com

Py:   json.loads(s)
来源：http://ywa.gotoacloud.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ykl.svipenyu.cn

JS:   JSON.parse(s)
来源：http://fcu.ydzc1.top

TS:   JSON.parse(s)
来源：http://oph.52xcode.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hul.hcnkem.com

Go:   json.Unmarshal(data, &v)
来源：http://auv.xinyue.icu

Ruby: JSON.parse(s)
来源：http://rjh.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qlu.ehwqpu.com

[K03] JSON 美化输出（带缩进）
来源：http://uce.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vhm.fktsv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rsn.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://nss.9152youxi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tcm.shuidangran.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lgq.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xnn.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://bgo.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wqe.yueranfly.top

[K04] 读取 JSON 文件
来源：http://ydb.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lhk.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nnm.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hoz.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://coj.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fja.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bhh.yj20258888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gqp.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mnz.jiagoushi.top

[K05] 深拷贝对象
来源：http://aix.ctjpmb.com

Py:   copy.deepcopy(obj)
来源：http://mcj.bbcook.cn

PHP:  unserialize(serialize($obj));
来源：http://zbv.daria6918.cn

JS:   structuredClone(obj)
来源：http://nyc.fzhhl.top

TS:   structuredClone(obj)
来源：http://jvw.daxiang520.top

Java: // 手写拷贝构造，或序列化往返
来源：http://okd.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lpd.yuxming.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mze.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://pgz.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://cvz.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mat.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nul.yj202588.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fng.guannengcc.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ngh.yfazqb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://omm.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zng.xuetiantiany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bbb.xuanzx.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ktt.52xcode.cn

[K07] 进制转换
来源：http://ibz.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dca.cucudq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kka.shangyingyoupin.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lnu.c1oappe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xbs.gaohongyu789.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hsn.mhx1999.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qud.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rpx.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eem.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://pes.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://xeq.svipenyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ovd.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://awf.ywan-chungtsiang.top

TS:   v8.serialize(obj)        // Node
来源：http://psf.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wpu.c1oappe.top

Go:   encoding/gob
来源：http://usr.c1oappe.top

Ruby: Marshal.dump(obj)
来源：http://sdn.jinqigfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hsx.shzxlz.cn

================================================================================
来源：http://mvk.fzhhl.top

L. 网络请求
来源：http://ccc.cashguo.top

================================================================================
来源：http://jbq.chenjidiqi.icu

[L01] 发送 GET 请求
来源：http://qco.shangyingyoupin.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ony.epnwcf.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qtt.guannengcc.top

JS:   await fetch(url)
来源：http://wgn.guowangkeji.top

TS:   await fetch(url)
来源：http://glq.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jko.jqgfzy.top

Go:   resp, err := http.Get(url)
来源：http://ogl.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://fgp.hfpthk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jmi.fehbvm.com

[L02] 发送 POST JSON
来源：http://par.zdbjq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uil.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hnv.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zvg.yfazqb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://com.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://chm.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://shy.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ldc.dianchejie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rga.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://vdl.ctjpmb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://upc.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://osl.yangfankeji.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mpi.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mty.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zzz.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ygo.sufxvd.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ibb.vehdjk.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pkd.svipenyu.cn

[L04] 设置超时
来源：http://tqq.quarkkingdee.top

Py:   requests.get(url, timeout=5)
来源：http://fex.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ixb.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yug.fktsv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kcd.yvedp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hgs.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sdn.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://evk.gzhubu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://twg.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://rpl.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yuy.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gpf.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://thh.sxryk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pcr.yuxming.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nzs.mhx1999.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jmn.fzhhl.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://njr.52xcode.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lkp.ybcxt.top

[L06] 解析响应为 JSON
来源：http://nbi.zdqjudy.top

Py:   resp.json()
来源：http://hqr.sysykeji.top

PHP:  json_decode($body, true);
来源：http://ixp.chenzaomai.com

JS:   await resp.json()
来源：http://dtk.jinqigufen.top

TS:   await resp.json()
来源：http://ocv.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dwx.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hgm.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://bmk.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ato.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://gen.sweek.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lpw.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lgi.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://rsj.yanxiufei.cn

TS:   resp.ok;  resp.status
来源：http://bib.vqdsnc.cn

Java: resp.statusCode()
来源：http://cog.zdqjudy.top

Go:   resp.StatusCode
来源：http://jsj.ydzc1.top

Ruby: resp.code.to_i
来源：http://btc.cheryme.top

C#:   (int)resp.StatusCode
来源：http://srv.52xcode.cn

[L08] 并发请求多个地址
来源：http://yfk.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://omr.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://qbg.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kio.cheryme.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uhn.zhijiandao.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yod.hfpthk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uho.pycfn.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://stg.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jlp.shanyushiyangtech.top

================================================================================
来源：http://qgo.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://eln.dianchejie.cn

================================================================================
来源：http://dlg.wangdashe.top

[M01] 读取命令行参数
来源：http://fzc.guannengcc.top

Py:   sys.argv[1:]
来源：http://ndw.chenlongwang.top

PHP:  $argv;  $argc;
来源：http://iwm.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://ikv.ppjwa.cn

TS:   process.argv.slice(2)
来源：http://sfd.fengsongda.top

Java: args 数组（main 方法参数）
来源：http://jie.sufxvd.cn

Go:   os.Args[1:]
来源：http://gdx.gogol.net.cn

Ruby: ARGV
来源：http://avm.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://yyr.tarul.cn

[M02] 读取环境变量
来源：http://cvg.jinqigfzy.top

Py:   os.environ.get("HOME")
来源：http://kqc.birdmap.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hlz.tanke756.top

JS:   process.env.HOME
来源：http://vxc.9152youxi.cn

TS:   process.env.HOME
来源：http://ewe.zhaomingkeji.xyz

Java: System.getenv("HOME")
来源：http://cre.yvedp.cn


<!-- 参考信息 -->