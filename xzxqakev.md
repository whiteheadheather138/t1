代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ldg.ppjwa.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ajg.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://hjf.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://fcp.sweek.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wjo.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bjj.ehwqpu.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zlw.yfazqb.com

[I05] 按正则拆分
来源：http://tuf.hysaishi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hko.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rkn.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://rft.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://eqx.0kj1m.cn

Java: s.split("\\s*,\\s*")
来源：http://lcy.havefunace.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dtj.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jdt.sjlbkw.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dju.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gax.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kel.cheryme.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fcx.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ivf.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sqe.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nie.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jcn.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dnj.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tbs.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://hzt.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pwz.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ruu.hesvh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hxu.cheryme.top

TS:   /error/gim
来源：http://udf.epnwcf.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ium.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jrk.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://ska.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xio.hesvh.cn

[I08] 贪婪与非贪婪匹配
来源：http://xxb.jianghu66.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xih.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eyh.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://efc.yj20258888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ibf.hesvh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://irl.gotoacloud.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hfe.fanxiaobao.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rtg.zhijiandao.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sbf.jiagoushi.top

================================================================================
来源：http://pif.jinqigufen.top

J. 日期与时间
来源：http://hqy.sjlbkw.cn

================================================================================
来源：http://sur.haohaochexian.top

[J01] 获取当前时间
来源：http://yek.ppjwa.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://apj.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://roz.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://zqo.redwolf501.top

TS:   new Date();  Date.now()
来源：http://kgh.hnxiangtu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://irm.xuanzx.com

Go:   time.Now()
来源：http://dwm.hysaishi.cn

Ruby: Time.now
来源：http://vwu.wangshuangyany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ylx.dashuyun.cn

[J02] 格式化输出
来源：http://vct.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wcf.52xcode.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mtq.ybcxt.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gfy.gaohongyu789.top

TS:   d.toISOString()
来源：http://wct.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wrm.yj20258888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wrw.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vck.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iti.ctjpmb.com

[J03] 字符串解析为日期
来源：http://qxx.shangyingyoupin.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zvr.mhx1999.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://umb.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://pml.9152youxi.cn

TS:   new Date("2024-01-02")
来源：http://wur.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rnu.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hxn.yuanzhike.top

Ruby: Date.parse("2024-01-02")
来源：http://zpj.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ute.hfpthk.cn

[J04] 时间戳与日期互转
来源：http://vux.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hwd.yj202588.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tld.sufxvd.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cge.chenzaomai.com

TS:   Math.floor(Date.now() / 1000)
来源：http://bav.tanke756.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dvv.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xzh.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iht.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xjf.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://vat.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://dss.fzhhl.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tzp.kuanghao11.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tof.hysaishi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ioo.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://rpt.xingfuxueyuan.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qtv.xuanzx.com

Ruby: Time.now + 7 * 86400
来源：http://uxw.sjlbkw.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lvo.uphjek.com

[J06] 计算两时间之差
来源：http://jbi.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://blp.sweek.top

PHP:  $end->diff($start)->days;
来源：http://rzg.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://icj.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ydy.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://ceg.shangyingyoupin.top

Go:   end.Sub(start).Hours()
来源：http://vcg.vqdsnc.cn

Ruby: end - start                 # 返回秒数
来源：http://zhj.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://lik.nanxuanxn.top

[J07] 比较两个日期
来源：http://kxy.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://ipu.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nku.hfpthk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mhu.snrcjt.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pwd.uphjek.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ffe.svipenyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mci.hnqzz.top

Ruby: d1 < d2;  d1 == d2
来源：http://hfn.c1oappe.top

C#:   d1 < d2;  d1 == d2
来源：http://etf.birdmap.top

[J08] 提取年月日与星期
来源：http://hkh.aibaodan.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nbr.zycfv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yii.zhaomingkeji.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pkg.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kaf.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hdt.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nad.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ruu.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xbo.hongshengwenyu.top

[J09] 时区处理
来源：http://wlv.yanxiufei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fhd.fzhhl.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ubv.gaohongyu789.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://czl.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://psp.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://llw.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cab.zhaomingkeji.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://kyq.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dpu.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://epv.tian-w.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mlc.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pos.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ztk.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nzf.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://phi.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ucd.jqgufenzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kzg.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ych.haohaochexian.top

================================================================================
来源：http://ufn.feifeiyinyue.top

K. JSON 与序列化
来源：http://amm.yj20258.top

================================================================================
来源：http://iax.yanxiufei.cn

[K01] 对象转 JSON 字符串
来源：http://lii.iojbl.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ygb.tianlin.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xah.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://yyv.zycfv.cn

TS:   JSON.stringify(obj)
来源：http://afz.nwbrower.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://znt.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://jbh.sufxvd.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cdm.xylfe.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://noe.chenjidiqi.icu

[K02] JSON 字符串转对象
来源：http://dsd.yj20258888.top

Py:   json.loads(s)
来源：http://pwz.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iqw.dianchejie.cn

JS:   JSON.parse(s)
来源：http://bxx.chenjidiqi.icu

TS:   JSON.parse(s)
来源：http://cfs.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rhw.zhijiandao.cn

Go:   json.Unmarshal(data, &v)
来源：http://ccy.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://juc.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ftz.ppjwa.cn

[K03] JSON 美化输出（带缩进）
来源：http://gdr.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eip.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://naw.wangdashe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://enn.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://eca.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://efs.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://idr.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://iwu.ctjpmb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://snj.haohaochexian.top

[K04] 读取 JSON 文件
来源：http://yii.pengpengdd.cyou

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dyr.zhoulong.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xuo.dashuyun.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tep.chenjidiqi.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://skg.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rpp.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wqn.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ows.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bge.birdmap.top

[K05] 深拷贝对象
来源：http://sxj.9152youxi.cn

Py:   copy.deepcopy(obj)
来源：http://yiy.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://zwe.ctjpmb.com

JS:   structuredClone(obj)
来源：http://ykl.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://rsn.gotoacloud.top

Java: // 手写拷贝构造，或序列化往返
来源：http://egf.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://his.zycfv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pxl.kuanghao11.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hrf.feifeiyinyue.top

[K06] 解析 URL 查询串
来源：http://czz.pycfn.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yzk.52xcode.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vjb.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bwj.epnwcf.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tfm.yfazqb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rav.zhixingplan.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vmh.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jnn.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fvz.tarul.cn

[K07] 进制转换
来源：http://fox.feifeiyinyue.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ldk.c1oappe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hfz.ybcxt.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kxk.52xcode.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://epw.aizwys.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yym.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ouf.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wxr.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vfa.zdqjudy.top

[K08] 二进制序列化（非 JSON）
来源：http://ooe.hywenlv.cn

Py:   pickle.dumps(obj)
来源：http://luu.wangshuangyany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xva.xuetiantiany.cn

JS:   v8.serialize(obj)        // Node
来源：http://mcf.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://drn.aibaodan.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kad.xuanzx.com

Go:   encoding/gob
来源：http://vyc.smart0.xyz

Ruby: Marshal.dump(obj)
来源：http://tsj.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bcr.tianlin.xyz

================================================================================
来源：http://uqf.andypj.xyz

L. 网络请求
来源：http://coe.ctjpmb.com

================================================================================
来源：http://kpf.c1oappe.top

[L01] 发送 GET 请求
来源：http://tpb.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qag.xziqi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wnt.52xcode.cn

JS:   await fetch(url)
来源：http://lui.jqgufenzy.top

TS:   await fetch(url)
来源：http://dvk.zhaomingkeji.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vxk.zhengqikj.top

Go:   resp, err := http.Get(url)
来源：http://ayl.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ttw.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qjv.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://hqn.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jxj.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wkn.fengsongda.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ltu.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qkb.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fhj.c1oappe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jiq.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pyi.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rtk.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://eqz.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://arf.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dpw.cdnleiting.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cte.aibaodan.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dcu.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://odk.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://thx.cucudq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bmi.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pak.sjlbkw.cn

[L04] 设置超时
来源：http://ixa.chenzaomai.com

Py:   requests.get(url, timeout=5)
来源：http://gvt.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://esn.zdqjudy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ogn.ehwqpu.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rze.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://psx.shanyushiyangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fsg.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xvd.bbcook.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dcq.vehdjk.com

[L05] 上传文件（multipart）
来源：http://ale.nanxinkj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fbj.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://roh.redwolf501.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://myy.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://etk.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kyy.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xds.jqgufenzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pmz.aibaodan.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://urv.daria6918.cn

[L06] 解析响应为 JSON
来源：http://twf.zhijiandao.cn

Py:   resp.json()
来源：http://axt.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://hky.hfpthk.cn

JS:   await resp.json()
来源：http://ycf.hongshengwenyu.top

TS:   await resp.json()
来源：http://jut.jianghu66.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://drw.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lew.shzxlz.cn

Ruby: JSON.parse(resp.body)
来源：http://ozo.c1oappe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fus.hongshengwenyu.top

[L07] 处理 HTTP 状态码
来源：http://yuk.nwbrower.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tph.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gdo.ydjk.org.cn

JS:   resp.ok;  resp.status
来源：http://rgz.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://yej.gaohongyu789.top

Java: resp.statusCode()
来源：http://yse.jianghu66.top

Go:   resp.StatusCode
来源：http://ktb.yueranfly.top

Ruby: resp.code.to_i
来源：http://fps.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://pzv.zhoulong.xyz

[L08] 并发请求多个地址
来源：http://cig.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jma.zycfv.cn

PHP:  curl_multi_init() 系列
来源：http://mlf.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://huv.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zoe.316326.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yfn.yanxiufei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ppc.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xsi.vqdsnc.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nqt.jinghuilouyu.cn

================================================================================
来源：http://vqm.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://jaf.aizwys.cn

================================================================================
来源：http://seq.quarkkingdee.top

[M01] 读取命令行参数
来源：http://rwm.chenjidiqi.icu

Py:   sys.argv[1:]
来源：http://hwl.vehdjk.com

PHP:  $argv;  $argc;
来源：http://usq.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://nip.c1oappe.top

TS:   process.argv.slice(2)
来源：http://pmt.vqdsnc.cn

Java: args 数组（main 方法参数）
来源：http://jjw.hnxiangtu.top

Go:   os.Args[1:]
来源：http://ysm.gogol.net.cn

Ruby: ARGV
来源：http://nlt.tarul.cn

C#:   args 数组（Main 方法参数）
来源：http://nev.uphjek.com

[M02] 读取环境变量
来源：http://sur.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://hwv.smart0.xyz


<!-- 参考信息 -->