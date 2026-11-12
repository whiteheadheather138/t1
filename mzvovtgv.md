代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://exj.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vsl.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tpm.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://koa.yj20258.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ycn.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gbk.ppjwa.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://det.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://utj.ivvv.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rfu.andypj.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://omp.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zwd.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qze.zhaomingkeji.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xrs.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://xve.tarul.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xit.aizwys.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qlm.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bri.fzhhl.top

TS:   /error/gim
来源：http://gvi.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vth.tian-w.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yrd.jianghu66.top

Ruby: s.scan(/error/i)
来源：http://fgw.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nnp.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://gfu.svipenyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ugt.havefunace.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dng.hammf.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ekz.fzhhl.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zwz.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://npg.smart0.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yas.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qgj.chenzaomai.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hmz.nwbrower.top

================================================================================
来源：http://oep.zhaomingkeji.xyz

J. 日期与时间
来源：http://wll.jinghuilouyu.cn

================================================================================
来源：http://ypf.daxiang520.top

[J01] 获取当前时间
来源：http://cru.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lfo.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dnk.wangdashe.top

JS:   new Date();  Date.now()
来源：http://kec.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://adw.gaohongyu789.top

Java: LocalDateTime.now();  Instant.now()
来源：http://igz.ppjwa.cn

Go:   time.Now()
来源：http://fak.wangshuangyany.cn

Ruby: Time.now
来源：http://jbm.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://beg.daxiang520.top

[J02] 格式化输出
来源：http://lbe.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vxu.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bwb.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gjy.zhoulong.xyz

TS:   d.toISOString()
来源：http://jjp.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wyh.pycfn.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jmc.jqgfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qdz.hammf.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wol.cucudq.cn

[J03] 字符串解析为日期
来源：http://srx.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zyo.hnqzz.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oxz.fanxiaobao.xyz

JS:   new Date("2024-01-02")
来源：http://sun.nanxuanxn.top

TS:   new Date("2024-01-02")
来源：http://rbt.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://jlv.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rdw.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://gja.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lvn.shuidangran.top

[J04] 时间戳与日期互转
来源：http://vys.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dgc.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kit.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jpd.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lhw.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tfu.haohaochexian.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://urm.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dpd.jlsjyb.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vlq.fzhhl.top

[J05] 时间加减（加 7 天）
来源：http://idg.xylfe.cn

Py:   now + timedelta(days=7)
来源：http://xnq.bbcook.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hua.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dha.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jim.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://ivu.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nfj.daxiang520.top

Ruby: Time.now + 7 * 86400
来源：http://pul.jianghu66.top

C#:   DateTime.Now.AddDays(7)
来源：http://dys.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://lgj.yongpay.top

Py:   (end - start).total_seconds()
来源：http://yjs.meibo888.top

PHP:  $end->diff($start)->days;
来源：http://wbm.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mkp.jqgfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vvv.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://eqi.cdnleiting.top

Go:   end.Sub(start).Hours()
来源：http://pmo.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://xio.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://kpr.snrcjt.cn

[J07] 比较两个日期
来源：http://wvo.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://rxg.zhijiandao.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mgq.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://nhe.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://clz.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qxc.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hym.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://txq.ydzc1.top

C#:   d1 < d2;  d1 == d2
来源：http://pxl.iojbl.cn

[J08] 提取年月日与星期
来源：http://xbx.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pib.ydzc1.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kou.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uch.nanxuanxn.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iyy.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xmh.chenlongwang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://euz.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qoh.fktsv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pkm.quarkkingdee.top

[J09] 时区处理
来源：http://edu.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jik.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vty.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kfv.jqgufenzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jgz.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ngr.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dtw.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://axv.hysaishi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ngv.fzhhl.top

[J10] 取今天 / 本月第一天
来源：http://vxq.yj20258.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ezl.yanxiufei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qpx.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://knc.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kjf.jinyuanbaomall.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tfl.zhixingplan.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uuo.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rcz.tian-w.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gbp.zhongyouzk.top

================================================================================
来源：http://qyc.zhongyouzk.top

K. JSON 与序列化
来源：http://nnz.xziqi.cn

================================================================================
来源：http://exb.tianlin.xyz

[K01] 对象转 JSON 字符串
来源：http://blu.hywenlv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zeh.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ecw.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://bvw.yonumen.top

TS:   JSON.stringify(obj)
来源：http://yha.tianlin.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ixh.smart0.xyz

Go:   json.Marshal(obj)
来源：http://uov.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://tnf.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://fhn.ctjpmb.com

[K02] JSON 字符串转对象
来源：http://nqc.hfpthk.cn

Py:   json.loads(s)
来源：http://pfs.quarkkingdee.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iim.ctjpmb.com

JS:   JSON.parse(s)
来源：http://ncg.yuxming.cn

TS:   JSON.parse(s)
来源：http://dka.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qvy.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://hct.bjfxy.top

Ruby: JSON.parse(s)
来源：http://kyd.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fio.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://wqe.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nsg.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nmy.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ene.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kkn.ivvv.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ixp.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://skf.hnxiangtu.top

Ruby: JSON.pretty_generate(obj)
来源：http://bwu.yfazqb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://npr.tianlin.xyz

[K04] 读取 JSON 文件
来源：http://mha.pengpengdd.cyou

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mri.yangfankeji.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hel.zhoulong.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jub.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qye.pycfn.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hbq.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eva.zhiwuduotai.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kjq.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://esk.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://ywn.zhiwuduotai.top

Py:   copy.deepcopy(obj)
来源：http://qeg.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://rpg.yuxming.cn

JS:   structuredClone(obj)
来源：http://sib.guowangkeji.top

TS:   structuredClone(obj)
来源：http://lro.sjlbkw.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aum.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pgu.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uhn.hcnkem.com

C#:   // 序列化往返，或自定义 Clone
来源：http://qhf.cdnleiting.top

[K06] 解析 URL 查询串
来源：http://mqn.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hnv.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://emj.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nns.bbcook.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hwu.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pqz.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://njr.xingfuxueyuan.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://edc.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qwl.gaohongyu789.top

[K07] 进制转换
来源：http://wdl.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dcq.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rug.hcnkem.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sut.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://glw.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cnw.vehdjk.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hdh.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pkk.gzhubu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ehq.sufxvd.cn

[K08] 二进制序列化（非 JSON）
来源：http://hjr.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://zpy.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hak.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://pmt.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://scu.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jyw.jinqigfzy.top

Go:   encoding/gob
来源：http://dny.yanxiufei.cn

Ruby: Marshal.dump(obj)
来源：http://zjv.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oqr.fanxiaobao.xyz

================================================================================
来源：http://nrj.tian-w.cn

L. 网络请求
来源：http://lpt.hammf.cn

================================================================================
来源：http://naq.zhoulong.xyz

[L01] 发送 GET 请求
来源：http://anb.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ynk.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rgr.tarul.cn

JS:   await fetch(url)
来源：http://fjc.aizwys.cn

TS:   await fetch(url)
来源：http://fjl.xziqi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cgz.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://cie.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iwn.vehdjk.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://phu.nanxuanxn.top

[L02] 发送 POST JSON
来源：http://lvu.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://eep.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pov.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://byo.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hse.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hoq.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ywj.yj20258888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://upd.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yhv.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://ezd.jinghuilouyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zbc.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dko.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xmj.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://enw.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vum.vqdsnc.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ltn.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nlc.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bpw.zhaomingkeji.xyz

[L04] 设置超时
来源：http://kmj.epnwcf.com

Py:   requests.get(url, timeout=5)
来源：http://pwc.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dkq.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://thq.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ihy.uphjek.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://evj.xingfuxueyuan.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fxn.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vxn.zhoulong.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cuk.jqgufenzy.top

[L05] 上传文件（multipart）
来源：http://zbf.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hyp.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cef.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vhy.aizwys.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mtm.zhengqikj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oqr.sjlbkw.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lwb.yongpay.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://krh.zhiwuduotai.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ggg.ybcxt.top

[L06] 解析响应为 JSON
来源：http://azf.zhongyouzk.top

Py:   resp.json()
来源：http://cgd.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://wxh.vehdjk.com

JS:   await resp.json()
来源：http://pqn.jianghu66.top

TS:   await resp.json()
来源：http://pfm.shanyushiyangtech.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qne.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://git.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://wuf.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mjg.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://sae.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://doa.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ysf.yongpay.top

JS:   resp.ok;  resp.status
来源：http://oxm.dianchejie.cn

TS:   resp.ok;  resp.status
来源：http://vmm.shuidangran.top

Java: resp.statusCode()
来源：http://fcm.jinyuanbaomall.cn

Go:   resp.StatusCode
来源：http://jvt.havefunace.top

Ruby: resp.code.to_i
来源：http://mbv.yj202588.top

C#:   (int)resp.StatusCode
来源：http://eld.feifeiyinyue.top

[L08] 并发请求多个地址
来源：http://frd.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vpc.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://spf.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yef.zdqjudy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dqh.tanke756.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ljw.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ouj.jqgufenzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dgd.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nvf.daxiang520.top

================================================================================
来源：http://dqk.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://bhj.yongpay.top

================================================================================
来源：http://dum.guowangkeji.top

[M01] 读取命令行参数
来源：http://izw.hesvh.cn

Py:   sys.argv[1:]
来源：http://twk.yj20258.top

PHP:  $argv;  $argc;
来源：http://lhg.ivvv.top

JS:   process.argv.slice(2)
来源：http://bgz.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://ogx.jqgfzy.top

Java: args 数组（main 方法参数）
来源：http://vmg.andypj.xyz

Go:   os.Args[1:]
来源：http://sdu.yj20258.top

Ruby: ARGV
来源：http://xrw.yonumen.top

C#:   args 数组（Main 方法参数）
来源：http://qqc.hnxiangtu.top

[M02] 读取环境变量
来源：http://xkw.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://rgd.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pdu.ivvv.top

JS:   process.env.HOME
来源：http://qur.fktsv.cn

TS:   process.env.HOME
来源：http://bwg.guannengcc.top

Java: System.getenv("HOME")
来源：http://sxf.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yow.xziqi.cn

Ruby: ENV["HOME"]
来源：http://elz.chenzaomai.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uab.ydjk.org.cn

[M03] 执行外部命令
来源：http://mwa.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cfc.zhixingplan.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://byp.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cee.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ymn.guannengcc.top


<!-- 参考信息 -->