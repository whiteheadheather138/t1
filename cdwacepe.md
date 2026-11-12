代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://wze.yanxiufei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dft.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://jwr.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fuw.aizwys.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qpj.cheryme.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://usy.aibaodan.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wku.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kbv.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://the.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eji.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ers.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zpf.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vpq.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://aft.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jzk.yanxiufei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rmq.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bkl.birdmap.top

TS:   /error/gim
来源：http://mnw.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wiu.zdqjudy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bug.bjfxy.top

Ruby: s.scan(/error/i)
来源：http://pdj.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gio.svipenyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://xol.zhongyouzk.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wdw.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rqc.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hag.aizwys.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pii.xuetiantiany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hqk.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nrq.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ohl.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://klg.wangshuangyany.cn

================================================================================
来源：http://pss.jinyuanbaomall.cn

J. 日期与时间
来源：http://pou.nanxuanxn.top

================================================================================
来源：http://fzi.zdqjudy.top

[J01] 获取当前时间
来源：http://czt.yj20258888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cni.9152youxi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://auf.zhengqikj.top

JS:   new Date();  Date.now()
来源：http://jpp.zdqjudy.top

TS:   new Date();  Date.now()
来源：http://qac.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sed.jinqigufen.top

Go:   time.Now()
来源：http://bwa.hnqzz.top

Ruby: Time.now
来源：http://cna.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fqs.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://iop.jiagoushi.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yei.shuidangran.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dwz.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tho.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://ejb.guowangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zdg.feifeiyinyue.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dme.gzhubu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hos.wangshuangyany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fyg.ydjk.org.cn

[J03] 字符串解析为日期
来源：http://rcb.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jkk.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bzm.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://inf.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://xuy.hongshengwenyu.top

Java: LocalDate.parse("2024-01-02")
来源：http://lnj.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uiy.hongshengwenyu.top

Ruby: Date.parse("2024-01-02")
来源：http://seg.zhijiandao.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rpw.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://sbs.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zkb.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bdq.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rcy.hywenlv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mwl.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ncm.nanxinkj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://leu.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ehc.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zha.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://nct.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://phn.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rri.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ltu.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dun.cdnleiting.top

Java: LocalDate.now().plusDays(7)
来源：http://ohv.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qfy.yj20258888.top

Ruby: Time.now + 7 * 86400
来源：http://mpg.cashguo.top

C#:   DateTime.Now.AddDays(7)
来源：http://fkf.hcnkem.com

[J06] 计算两时间之差
来源：http://nyk.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://rsk.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://eik.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://njb.tianlin.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kyt.uphjek.com

Java: Duration.between(start, end).toSeconds()
来源：http://pzu.smart0.xyz

Go:   end.Sub(start).Hours()
来源：http://aro.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://pwa.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://igi.haohaochexian.top

[J07] 比较两个日期
来源：http://uio.nanxuanxn.top

Py:   d1 < d2;  d1 == d2
来源：http://dok.fzhhl.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ooy.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://xdq.hesvh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://alh.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gjc.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ray.ydjk.org.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fom.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://jdp.birdmap.top

[J08] 提取年月日与星期
来源：http://tbo.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://llf.xuanzx.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://idf.pengpengdd.cyou

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rrv.sysykeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qaj.yj202588.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ovq.fehbvm.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://krz.hysaishi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mdx.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pvc.chenzaomai.com

[J09] 时区处理
来源：http://yzc.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ssc.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://whh.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wew.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hvs.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ere.mhx1999.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://inf.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qty.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sng.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://vkw.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zqc.cdnleiting.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eky.yfazqb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mhp.shanyushiyangtech.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zrx.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xvj.xinyue.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fvg.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yqi.smart0.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ref.sufxvd.cn

================================================================================
来源：http://vtx.chenlongwang.top

K. JSON 与序列化
来源：http://oub.smart0.xyz

================================================================================
来源：http://lfe.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://enc.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mhq.ydjk.org.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wme.jinqigufen.top

JS:   JSON.stringify(obj)
来源：http://mlk.hnqzz.top

TS:   JSON.stringify(obj)
来源：http://ibj.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zmy.hesvh.cn

Go:   json.Marshal(obj)
来源：http://rut.xziqi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nck.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ddy.shuidangran.top

[K02] JSON 字符串转对象
来源：http://ipy.sxryk.cn

Py:   json.loads(s)
来源：http://lsz.fzhhl.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rzk.sweek.top

JS:   JSON.parse(s)
来源：http://dwt.cashguo.top

TS:   JSON.parse(s)
来源：http://ici.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kqt.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://rld.cashguo.top

Ruby: JSON.parse(s)
来源：http://lfh.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://upn.haohaochexian.top

[K03] JSON 美化输出（带缩进）
来源：http://vrj.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mvk.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vlp.zhaomingkeji.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://ole.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rlj.hcnkem.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gxv.shanyushiyangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bpw.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://qgc.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ecc.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://hdx.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dtj.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://llh.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rxk.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kdk.shanyushiyangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xoe.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ybn.sxryk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://saf.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://osn.gogol.net.cn

[K05] 深拷贝对象
来源：http://qkm.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://qwj.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://ddt.chenjidiqi.icu

JS:   structuredClone(obj)
来源：http://pkp.daxiang520.top

TS:   structuredClone(obj)
来源：http://fol.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bec.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fax.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fbx.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://szi.tian-w.cn

[K06] 解析 URL 查询串
来源：http://hzd.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hjc.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mji.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uzg.iojbl.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xhp.shangyingyoupin.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kxk.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://tqq.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xvy.ctjpmb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uei.cashguo.top

[K07] 进制转换
来源：http://vnn.tian-w.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hgr.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://onr.kuanghao11.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rhs.zhixingplan.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pei.jinqigfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hmn.shuidangran.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bnk.yfazqb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xgq.chenzaomai.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vol.birdmap.top

[K08] 二进制序列化（非 JSON）
来源：http://swn.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://dyc.zhaomingkeji.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://izv.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://cws.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://rok.yueranfly.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ixe.iojbl.cn

Go:   encoding/gob
来源：http://azn.hongshengwenyu.top

Ruby: Marshal.dump(obj)
来源：http://ill.ivvv.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ckf.zdqjudy.top

================================================================================
来源：http://zqc.daria6918.cn

L. 网络请求
来源：http://kel.52xcode.cn

================================================================================
来源：http://zun.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://kup.yangfankeji.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aeo.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vma.sysykeji.top

JS:   await fetch(url)
来源：http://qjp.cqqwz.cn

TS:   await fetch(url)
来源：http://sqi.bbcook.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yzw.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://jht.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nbt.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fod.guowangkeji.top

[L02] 发送 POST JSON
来源：http://xcg.andypj.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://fqy.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jbc.epnwcf.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vap.52xcode.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pam.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lkw.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://laa.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://npo.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://len.gzhubu.top

[L03] 设置自定义请求头
来源：http://tqk.xinyue.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sql.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://puj.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://agc.shanyushiyangtech.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jta.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oyt.hnxiangtu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://unr.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fkw.havefunace.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lmr.zhoulong.xyz

[L04] 设置超时
来源：http://udt.svipenyu.cn

Py:   requests.get(url, timeout=5)
来源：http://rou.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mvd.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xlt.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nwd.feifeiyinyue.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://asi.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jea.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://onx.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bew.redwolf501.top

[L05] 上传文件（multipart）
来源：http://qtt.cashguo.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wwl.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nwq.bbcook.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bfk.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rxc.mhx1999.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vgq.chenzaomai.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jsw.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fbp.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tan.guannengcc.top

[L06] 解析响应为 JSON
来源：http://iob.sxryk.cn

Py:   resp.json()
来源：http://paz.c1oappe.top

PHP:  json_decode($body, true);
来源：http://urp.kuanghao11.cn

JS:   await resp.json()
来源：http://aoz.yueranfly.top

TS:   await resp.json()
来源：http://afb.gaohongyu789.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wqs.svipenyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lrz.shzxlz.cn

Ruby: JSON.parse(resp.body)
来源：http://qvw.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://emv.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://nkw.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oxr.xinyue.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ona.zhaomingkeji.xyz

JS:   resp.ok;  resp.status
来源：http://ypy.meibo888.top

TS:   resp.ok;  resp.status
来源：http://yih.shangyingyoupin.top

Java: resp.statusCode()
来源：http://xih.mhx1999.top

Go:   resp.StatusCode
来源：http://jtu.shanyushiyangkeji.top

Ruby: resp.code.to_i
来源：http://udy.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://pki.hesvh.cn

[L08] 并发请求多个地址
来源：http://lyv.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oxk.jinghuilouyu.cn

PHP:  curl_multi_init() 系列
来源：http://ipk.chenjidiqi.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dtu.yuxming.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://asg.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cju.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sxh.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ssc.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gti.hnqzz.top

================================================================================
来源：http://erx.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://cvh.tanke756.top

================================================================================
来源：http://ahi.birdmap.top

[M01] 读取命令行参数
来源：http://zln.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://enf.fzhhl.top

PHP:  $argv;  $argc;
来源：http://yrf.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://liw.xuanzx.com

TS:   process.argv.slice(2)
来源：http://zqi.daxiang520.top

Java: args 数组（main 方法参数）
来源：http://rli.0kj1m.cn

Go:   os.Args[1:]
来源：http://cjh.feifeiyinyue.top

Ruby: ARGV
来源：http://pmb.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://qtv.zhoulong.xyz

[M02] 读取环境变量
来源：http://woy.haohaochexian.top

Py:   os.environ.get("HOME")
来源：http://cvp.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vzi.chenjidiqi.icu

JS:   process.env.HOME
来源：http://lrx.xziqi.cn

TS:   process.env.HOME
来源：http://kgg.yj20258888.top

Java: System.getenv("HOME")
来源：http://nms.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://heg.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://zpm.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tlw.xuetiantiany.cn

[M03] 执行外部命令
来源：http://ytr.svipenyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fna.zhixingplan.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kyv.ivvv.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cne.dianchejie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nok.hysaishi.cn


<!-- 参考信息 -->