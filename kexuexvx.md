代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pyi.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wrh.mhx1999.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jrt.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hdx.yanxiufei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://urk.zhoulong.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kvk.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tca.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rms.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gcp.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://qzr.ywan-chungtsiang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eiy.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zow.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://awy.hesvh.cn

TS:   /error/gim
来源：http://nhk.zycfv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vfn.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tcj.jlsjyb.cn

Ruby: s.scan(/error/i)
来源：http://yyo.birdmap.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pki.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://voz.cashguo.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mdg.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cbd.yj20258.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xhg.hfpthk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bsa.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qsy.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tru.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fpi.zdbjq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iqe.sxryk.cn

================================================================================
来源：http://dcn.svipenyu.cn

J. 日期与时间
来源：http://urj.jinyuanbaomall.cn

================================================================================
来源：http://gdj.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://wda.epnwcf.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://tlw.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vbv.fanxiaobao.xyz

JS:   new Date();  Date.now()
来源：http://erw.vqdsnc.cn

TS:   new Date();  Date.now()
来源：http://hec.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jfg.shangyingyoupin.top

Go:   time.Now()
来源：http://mbc.hnqzz.top

Ruby: Time.now
来源：http://trq.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iwn.cqqwz.cn

[J02] 格式化输出
来源：http://bsm.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ebp.shanyushiyangtech.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rln.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://niv.bbcook.cn

TS:   d.toISOString()
来源：http://pgt.hywenlv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fib.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jjq.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ivu.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gpi.zdqjudy.top

[J03] 字符串解析为日期
来源：http://lzk.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zyo.tianlin.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ajm.birdmap.top

JS:   new Date("2024-01-02")
来源：http://ung.wangdashe.top

TS:   new Date("2024-01-02")
来源：http://nzo.vqdsnc.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jdh.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tqj.zhixingplan.top

Ruby: Date.parse("2024-01-02")
来源：http://zss.cqqwz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://afk.0kj1m.cn

[J04] 时间戳与日期互转
来源：http://xgo.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fbg.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vcf.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jmx.guannengcc.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zfy.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pvf.yj20258.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vfd.vqdsnc.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://atc.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zpr.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://cvj.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://wkh.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ycn.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lpa.svipenyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nvr.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://cdc.nanxinkj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tus.yuanzhike.top

Ruby: Time.now + 7 * 86400
来源：http://mij.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://dxw.zdbjq.cn

[J06] 计算两时间之差
来源：http://jmy.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://lgk.vqdsnc.cn

PHP:  $end->diff($start)->days;
来源：http://oed.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ism.gotoacloud.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hpw.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://siw.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://ykl.haohaochexian.top

Ruby: end - start                 # 返回秒数
来源：http://lau.fzhhl.top

C#:   (end - start).TotalSeconds
来源：http://mhg.zhixingplan.top

[J07] 比较两个日期
来源：http://xqg.fktsv.cn

Py:   d1 < d2;  d1 == d2
来源：http://jyh.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jna.gotoacloud.top

JS:   d1.getTime() < d2.getTime()
来源：http://nla.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xam.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dtd.sxryk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aft.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cyy.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://bmi.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://fsa.ywan-chungtsiang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fjw.ydjk.org.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tlo.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nui.xingfuxueyuan.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ugg.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jfr.gaohongyu789.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jnc.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://osp.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cqv.nanxuanxn.top

[J09] 时区处理
来源：http://nyl.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bsx.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pxb.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lzg.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://psf.yueranfly.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bow.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rvg.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qeh.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cey.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://oyz.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zxb.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oes.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lia.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pho.xuanzx.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://coy.jlsjyb.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bvv.ywan-chungtsiang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nue.xylfe.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uro.smart0.xyz

================================================================================
来源：http://oth.shzxlz.cn

K. JSON 与序列化
来源：http://xur.guowangkeji.top

================================================================================
来源：http://yjx.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://kjc.snrcjt.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://buv.9152youxi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pmp.hammf.cn

JS:   JSON.stringify(obj)
来源：http://dgs.jinqigufen.top

TS:   JSON.stringify(obj)
来源：http://fnx.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gns.yj20258.top

Go:   json.Marshal(obj)
来源：http://hop.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xrz.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vfh.zhijiandao.cn

[K02] JSON 字符串转对象
来源：http://ofd.yuxming.cn

Py:   json.loads(s)
来源：http://lzk.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://srb.fanxiaobao.xyz

JS:   JSON.parse(s)
来源：http://rvl.cheryme.top

TS:   JSON.parse(s)
来源：http://hnx.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://erd.feifeiyinyue.top

Go:   json.Unmarshal(data, &v)
来源：http://lvu.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://vkt.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qby.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://zou.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jyd.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://adt.hesvh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mte.c1oappe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zxf.zhijiandao.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uiy.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mci.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://syu.redwolf501.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dxf.sufxvd.cn

[K04] 读取 JSON 文件
来源：http://lzo.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zvn.yfazqb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bgt.redwolf501.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ecz.ybcxt.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://evn.wangshuangyany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://akn.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jmw.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cke.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ekc.hammf.cn

[K05] 深拷贝对象
来源：http://kdl.zhixingplan.top

Py:   copy.deepcopy(obj)
来源：http://hfp.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://ysc.pycfn.com

JS:   structuredClone(obj)
来源：http://qei.cdnleiting.top

TS:   structuredClone(obj)
来源：http://xwo.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://akf.yvedp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://loa.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://opb.snrcjt.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wlg.bbcook.cn

[K06] 解析 URL 查询串
来源：http://fyb.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://plz.hesvh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xqa.daxiang520.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vtj.sweek.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nqe.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dir.zhiwuduotai.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://akv.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dmm.hnqzz.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hms.xylfe.cn

[K07] 进制转换
来源：http://mil.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yoa.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vwl.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wyc.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vql.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://geq.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bgr.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bql.sjlbkw.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bao.redwolf501.top

[K08] 二进制序列化（非 JSON）
来源：http://mbw.xuetiantiany.cn

Py:   pickle.dumps(obj)
来源：http://vhs.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://hxn.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://ijq.nanxinkj.top

TS:   v8.serialize(obj)        // Node
来源：http://fug.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ejk.tarul.cn

Go:   encoding/gob
来源：http://cwy.guannengcc.top

Ruby: Marshal.dump(obj)
来源：http://wpr.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xam.9152youxi.cn

================================================================================
来源：http://nse.tarul.cn

L. 网络请求
来源：http://xer.jqgfzy.top

================================================================================
来源：http://gmn.chenzaomai.com

[L01] 发送 GET 请求
来源：http://xla.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xzc.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dmv.sysykeji.top

JS:   await fetch(url)
来源：http://ozh.gzhubu.top

TS:   await fetch(url)
来源：http://nyi.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dlp.snrcjt.cn

Go:   resp, err := http.Get(url)
来源：http://guj.hywenlv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hpt.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gwp.guowangkeji.top

[L02] 发送 POST JSON
来源：http://ycw.xylfe.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wig.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lsx.zhengqikj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ica.fktsv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tea.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://whq.smart0.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ivl.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ycq.xinyue.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mlg.hcnkem.com

[L03] 设置自定义请求头
来源：http://bli.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ywj.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lck.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iyj.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qij.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tkv.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nqq.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ism.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://drr.feifeiyinyue.top

[L04] 设置超时
来源：http://ttl.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://lsa.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tno.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blt.9152youxi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nvm.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://unh.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dtp.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dnc.pycfn.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rqt.tanke756.top

[L05] 上传文件（multipart）
来源：http://hgg.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oug.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kby.316326.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lms.aizwys.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dhz.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://die.xingfuxueyuan.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ahm.chenzaomai.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rvw.zhongyouzk.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://asy.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://vuk.guannengcc.top

Py:   resp.json()
来源：http://sjt.xinyue.icu

PHP:  json_decode($body, true);
来源：http://wah.fanxiaobao.xyz

JS:   await resp.json()
来源：http://gqa.yueranfly.top

TS:   await resp.json()
来源：http://tum.vqdsnc.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wnh.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iew.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://zel.shuidangran.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xzl.sxryk.cn

[L07] 处理 HTTP 状态码
来源：http://ipn.cdnleiting.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dmo.ivvv.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iaa.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://xzq.fehbvm.com

TS:   resp.ok;  resp.status
来源：http://bec.guannengcc.top

Java: resp.statusCode()
来源：http://ktz.hnxiangtu.top

Go:   resp.StatusCode
来源：http://cwb.zdqjudy.top

Ruby: resp.code.to_i
来源：http://udo.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://gke.yongpay.top

[L08] 并发请求多个地址
来源：http://amt.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iza.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://sep.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kgd.sweek.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hkb.316326.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://esk.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qki.hywenlv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hgn.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zbq.yangfankeji.com

================================================================================
来源：http://nve.yvedp.cn

M. 命令行 / 进程 / 环境
来源：http://fme.tarul.cn

================================================================================
来源：http://fxi.yonumen.top

[M01] 读取命令行参数
来源：http://egv.yvedp.cn

Py:   sys.argv[1:]
来源：http://hco.xuanzx.com

PHP:  $argv;  $argc;
来源：http://hxl.iojbl.cn

JS:   process.argv.slice(2)
来源：http://fdb.jqgfzy.top

TS:   process.argv.slice(2)
来源：http://txt.ivvv.top

Java: args 数组（main 方法参数）
来源：http://qng.nwbrower.top

Go:   os.Args[1:]
来源：http://avu.jyoumei.cn

Ruby: ARGV
来源：http://tvf.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://kwj.svipenyu.cn

[M02] 读取环境变量
来源：http://uji.jianghu66.top

Py:   os.environ.get("HOME")
来源：http://zrc.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zow.316326.xyz

JS:   process.env.HOME
来源：http://efy.daxiang520.top

TS:   process.env.HOME
来源：http://jgd.aibaodan.cn

Java: System.getenv("HOME")
来源：http://vmk.hywenlv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gbe.epnwcf.com

Ruby: ENV["HOME"]
来源：http://mgu.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aan.pengpengdd.cyou

[M03] 执行外部命令
来源：http://aey.zycfv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zky.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yur.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vis.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dzp.zhiwuduotai.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lvq.xingfuxueyuan.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://wnl.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://nuk.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://gnc.gaohongyu789.top


<!-- 参考信息 -->