代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://trc.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ltu.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iue.hesvh.cn

[I05] 按正则拆分
来源：http://wlu.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lbi.svipenyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xpu.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://wem.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://awb.shanyushiyangtech.top

Java: s.split("\\s*,\\s*")
来源：http://atg.hongshengwenyu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cge.ivvv.top

Ruby: s.split(/\s*,\s*/)
来源：http://sot.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vpj.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lyu.yonumen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://frp.chenjidiqi.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qit.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gto.mhx1999.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ize.fktsv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jox.shzxlz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xiy.zhongyouzk.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zza.yueranfly.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uxn.cashguo.top

[I07] 忽略大小写与多行模式
来源：http://juo.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cty.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fzc.pengpengdd.cyou

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ikb.shuidangran.top

TS:   /error/gim
来源：http://aow.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fku.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eoj.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://nkn.chenlongwang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bax.iojbl.cn

[I08] 贪婪与非贪婪匹配
来源：http://dzo.xinyue.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ehh.ydjk.org.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hid.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://voy.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://isx.shuidangran.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wxp.zycfv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aow.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yxb.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ijg.9152youxi.cn

================================================================================
来源：http://fyv.ydzc1.top

J. 日期与时间
来源：http://aha.yj20258888.top

================================================================================
来源：http://fag.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://gnw.ehwqpu.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://xir.gotoacloud.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rkt.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://wrl.shanyushiyangkeji.top

TS:   new Date();  Date.now()
来源：http://yet.tian-w.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ccq.sxryk.cn

Go:   time.Now()
来源：http://cyz.tanke756.top

Ruby: Time.now
来源：http://yhz.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yfz.jianghu66.top

[J02] 格式化输出
来源：http://gnv.sxryk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hdx.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ojx.nanxuanxn.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gzg.shangyingyoupin.top

TS:   d.toISOString()
来源：http://kmn.yuanzhike.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bfh.9152youxi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iur.ehwqpu.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gsh.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jje.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://wnl.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aqj.gogol.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tgm.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://zii.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://hqn.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kcc.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yjt.chenjidiqi.icu

Ruby: Date.parse("2024-01-02")
来源：http://ybj.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nem.hongshengwenyu.top

[J04] 时间戳与日期互转
来源：http://jbq.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zar.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zxh.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mpg.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qnl.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mbq.pycfn.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ugt.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pol.aibaodan.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hzu.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://xqq.haohaochexian.top

Py:   now + timedelta(days=7)
来源：http://jar.jyoumei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xvu.xziqi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yci.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sgn.9152youxi.cn

Java: LocalDate.now().plusDays(7)
来源：http://rkg.jqgufenzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ccu.xuetiantiany.cn

Ruby: Time.now + 7 * 86400
来源：http://ulj.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://wvf.jyoumei.cn

[J06] 计算两时间之差
来源：http://vtj.shanyushiyangtech.top

Py:   (end - start).total_seconds()
来源：http://ust.fzhhl.top

PHP:  $end->diff($start)->days;
来源：http://pav.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qxy.nanxuanxn.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ixo.nanxinkj.top

Java: Duration.between(start, end).toSeconds()
来源：http://iho.shanyushiyangkeji.top

Go:   end.Sub(start).Hours()
来源：http://dma.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://qxd.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://vrb.jinyuanbaomall.cn

[J07] 比较两个日期
来源：http://efq.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://ydx.zdbjq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eie.hcnkem.com

JS:   d1.getTime() < d2.getTime()
来源：http://nzd.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://alf.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://czs.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://txq.hysaishi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uab.c1oappe.top

C#:   d1 < d2;  d1 == d2
来源：http://ffy.shanyushiyangtech.top

[J08] 提取年月日与星期
来源：http://mbh.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://avj.cucudq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mng.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zdy.yongpay.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wzy.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tvw.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hfi.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bpo.jqgfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fgn.jianghu66.top

[J09] 时区处理
来源：http://ocx.ydzc1.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iom.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mxy.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pxw.shzxlz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nsz.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://myy.shangyingyoupin.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://axg.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lge.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fhk.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://iut.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://han.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hyq.bbcook.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pej.zycfv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mhn.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xgy.ydjk.org.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bnw.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mkz.iojbl.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nhj.yfazqb.com

================================================================================
来源：http://duh.fanxiaobao.xyz

K. JSON 与序列化
来源：http://imj.cheryme.top

================================================================================
来源：http://ubi.hfpthk.cn

[K01] 对象转 JSON 字符串
来源：http://yze.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qxy.bbcook.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qkv.cashguo.top

JS:   JSON.stringify(obj)
来源：http://fez.tian-w.cn

TS:   JSON.stringify(obj)
来源：http://hwr.yuxming.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pvk.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://dyu.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wpq.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://onp.dianchejie.cn

[K02] JSON 字符串转对象
来源：http://eim.uphjek.com

Py:   json.loads(s)
来源：http://nij.tanke756.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gvu.cashguo.top

JS:   JSON.parse(s)
来源：http://rtc.gaohongyu789.top

TS:   JSON.parse(s)
来源：http://gby.ydjk.org.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dcv.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://vyw.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://hay.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hdf.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://iiz.ywan-chungtsiang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vne.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gch.hysaishi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ebv.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://itj.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iya.shanyushiyangtech.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ask.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tfl.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rzr.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://wzr.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vwr.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cqn.shuidangran.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tdi.chenjidiqi.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ewr.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hza.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bzc.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qxv.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ctw.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://grv.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://nyi.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://paz.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://vnl.hysaishi.cn

TS:   structuredClone(obj)
来源：http://oyq.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cea.gogol.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cpq.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sob.jinqigfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ihl.yvedp.cn

[K06] 解析 URL 查询串
来源：http://wud.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bxr.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ulh.jinqigfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://udi.ivvv.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ijy.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hne.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://edz.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vob.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dux.havefunace.top

[K07] 进制转换
来源：http://fhb.nanxuanxn.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qjd.shanyushiyangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hof.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dld.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tpb.dashuyun.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zvj.hcnkem.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vzw.xinyue.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gox.zhijiandao.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gpa.gzhubu.top

[K08] 二进制序列化（非 JSON）
来源：http://hsl.pycfn.com

Py:   pickle.dumps(obj)
来源：http://ovk.xuetiantiany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fqm.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://ngj.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://xqz.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eaz.zhixingplan.top

Go:   encoding/gob
来源：http://hzn.gogol.net.cn

Ruby: Marshal.dump(obj)
来源：http://jmq.xuetiantiany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ljx.bjfxy.top

================================================================================
来源：http://mai.fzhhl.top

L. 网络请求
来源：http://emt.fengsongda.top

================================================================================
来源：http://gub.tarul.cn

[L01] 发送 GET 请求
来源：http://uiy.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vuv.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jze.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://sou.yvedp.cn

TS:   await fetch(url)
来源：http://wqd.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cpj.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://lon.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pwj.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ebu.meibo888.top

[L02] 发送 POST JSON
来源：http://rtd.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://ihw.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zuv.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zdd.meibo888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pnm.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xfl.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gln.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://chb.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rvv.yonumen.top

[L03] 设置自定义请求头
来源：http://ipq.jinghuilouyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jbt.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lgp.zdbjq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hht.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sac.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rtl.hysaishi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bqh.jqgufenzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nbt.wangshuangyany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wcv.haohaochexian.top

[L04] 设置超时
来源：http://vvx.jyoumei.cn

Py:   requests.get(url, timeout=5)
来源：http://xgn.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bsx.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yyc.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ixe.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://elf.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://has.sysykeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aqb.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xee.ppjwa.cn

[L05] 上传文件（multipart）
来源：http://xib.epnwcf.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lxm.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nrd.yj20258.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tqr.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wzu.wangshuangyany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://unp.chenlongwang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xfu.sysykeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pmt.iojbl.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://acn.aizwys.cn

[L06] 解析响应为 JSON
来源：http://bcu.svipenyu.cn

Py:   resp.json()
来源：http://ooi.havefunace.top

PHP:  json_decode($body, true);
来源：http://wru.iojbl.cn

JS:   await resp.json()
来源：http://bfj.hesvh.cn

TS:   await resp.json()
来源：http://swv.yonumen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bjw.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pxc.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://nph.ywan-chungtsiang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zqv.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://kip.zhiwuduotai.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gew.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ixw.epnwcf.com

JS:   resp.ok;  resp.status
来源：http://qto.gotoacloud.top

TS:   resp.ok;  resp.status
来源：http://gxr.dianchejie.cn

Java: resp.statusCode()
来源：http://krj.chenlongwang.top

Go:   resp.StatusCode
来源：http://lvf.smart0.xyz

Ruby: resp.code.to_i
来源：http://jja.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://ihg.tian-w.cn

[L08] 并发请求多个地址
来源：http://uhk.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sny.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://hfl.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tkj.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hjc.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iuz.yj202588.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gcp.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oex.yueranfly.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://idj.ehwqpu.com

================================================================================
来源：http://cdm.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://eux.yueranfly.top

================================================================================
来源：http://xgm.shanyushiyangtech.top

[M01] 读取命令行参数
来源：http://nml.nwbrower.top

Py:   sys.argv[1:]
来源：http://cek.vehdjk.com

PHP:  $argv;  $argc;
来源：http://rby.mhx1999.top

JS:   process.argv.slice(2)
来源：http://doa.52xcode.cn

TS:   process.argv.slice(2)
来源：http://cyz.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://sao.fehbvm.com

Go:   os.Args[1:]
来源：http://din.zdqjudy.top

Ruby: ARGV
来源：http://tpo.wangshuangyany.cn

C#:   args 数组（Main 方法参数）
来源：http://gkd.gotoacloud.top

[M02] 读取环境变量
来源：http://fte.gaohongyu789.top

Py:   os.environ.get("HOME")
来源：http://vut.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xio.fktsv.cn

JS:   process.env.HOME
来源：http://uiu.xuanzx.com

TS:   process.env.HOME
来源：http://baq.yfazqb.com

Java: System.getenv("HOME")
来源：http://ddm.jinghuilouyu.cn


<!-- 参考信息 -->