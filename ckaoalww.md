代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://pdu.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hoc.hfpthk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ejo.zhengqikj.top

[I05] 按正则拆分
来源：http://bha.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://slk.cucudq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jht.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://vys.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://phb.xinyue.icu

Java: s.split("\\s*,\\s*")
来源：http://xzl.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dyq.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://vnq.jyoumei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mfv.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pnr.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dif.sweek.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mgh.pengpengdd.cyou

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bjm.hfpthk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://csf.dianchejie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://koa.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://njk.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://npy.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nsv.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://qrr.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cjm.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qpd.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ikq.yj20258.top

TS:   /error/gim
来源：http://jlx.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pbp.jianghu66.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dmy.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://xey.shanyushiyangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bzb.cheryme.top

[I08] 贪婪与非贪婪匹配
来源：http://hpb.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oaa.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://udp.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cuc.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://acc.hywenlv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dng.jinqigfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vrt.fanxiaobao.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ezn.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lrt.yonumen.top

================================================================================
来源：http://nrl.shuidangran.top

J. 日期与时间
来源：http://qsz.ydjk.org.cn

================================================================================
来源：http://tkr.yanxiufei.cn

[J01] 获取当前时间
来源：http://gmr.chenzaomai.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://gns.xingfuxueyuan.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ajv.uphjek.com

JS:   new Date();  Date.now()
来源：http://pvd.sufxvd.cn

TS:   new Date();  Date.now()
来源：http://vnh.hesvh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uwp.yj20258888.top

Go:   time.Now()
来源：http://rvk.xylfe.cn

Ruby: Time.now
来源：http://dyd.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qbz.cqqwz.cn

[J02] 格式化输出
来源：http://tiy.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mcx.yonumen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eub.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dyv.xuetiantiany.cn

TS:   d.toISOString()
来源：http://xhi.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rbc.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ixn.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vhk.hywenlv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yyb.jianghu66.top

[J03] 字符串解析为日期
来源：http://xzn.epnwcf.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eid.daxiang520.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rdp.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://skz.mhx1999.top

TS:   new Date("2024-01-02")
来源：http://zjb.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fbj.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cmf.birdmap.top

Ruby: Date.parse("2024-01-02")
来源：http://olh.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bdu.pengpengdd.cyou

[J04] 时间戳与日期互转
来源：http://twc.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://egz.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bop.aibaodan.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lmb.bjfxy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ffx.redwolf501.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://edw.jiagoushi.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://myd.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ubb.mhx1999.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://red.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://qlb.haohaochexian.top

Py:   now + timedelta(days=7)
来源：http://bqh.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sze.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uns.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xea.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://yib.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ssj.aibaodan.cn

Ruby: Time.now + 7 * 86400
来源：http://tsu.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://zqc.jinyuanbaomall.cn

[J06] 计算两时间之差
来源：http://cyr.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://wau.fzhhl.top

PHP:  $end->diff($start)->days;
来源：http://lld.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://thq.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zdx.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hjo.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://mxn.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://rgi.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://ecj.vqdsnc.cn

[J07] 比较两个日期
来源：http://sns.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://xms.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hjf.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://wiw.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://pnu.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qoi.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yvw.uphjek.com

Ruby: d1 < d2;  d1 == d2
来源：http://coe.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://hbv.bjfxy.top

[J08] 提取年月日与星期
来源：http://ggn.wangshuangyany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dpg.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xqy.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pyf.mhx1999.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pwo.fzhhl.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dfx.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://chp.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vrl.kuanghao11.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bzp.316326.xyz

[J09] 时区处理
来源：http://cvk.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bvo.yonumen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zsj.uphjek.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vsq.cheryme.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nxp.ydzc1.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gnb.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://stl.jinyuanbaomall.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://huw.birdmap.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hcn.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://ktq.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://bcb.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pnb.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://deq.xuanzx.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ymi.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ott.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gev.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bvp.xylfe.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://azo.vehdjk.com

================================================================================
来源：http://awe.yueranfly.top

K. JSON 与序列化
来源：http://kdb.9152youxi.cn

================================================================================
来源：http://upf.chenjidiqi.icu

[K01] 对象转 JSON 字符串
来源：http://mhu.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hre.yuxming.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gai.yj202588.top

JS:   JSON.stringify(obj)
来源：http://nyg.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://qay.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://atb.shanyushiyangkeji.top

Go:   json.Marshal(obj)
来源：http://qji.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://oij.ppjwa.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xwa.zhixingplan.top

[K02] JSON 字符串转对象
来源：http://dvd.cashguo.top

Py:   json.loads(s)
来源：http://uyv.jlsjyb.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://acq.fzhhl.top

JS:   JSON.parse(s)
来源：http://xzv.bbcook.cn

TS:   JSON.parse(s)
来源：http://wfw.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ctp.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://hcw.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://nam.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tih.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://efc.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ztx.hfpthk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rdj.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ddx.tarul.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sqa.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ash.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ear.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://dsp.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xro.yuxming.cn

[K04] 读取 JSON 文件
来源：http://kbs.daxiang520.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://plo.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gkt.havefunace.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://igd.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ife.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fmb.zdqjudy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vcb.hongshengwenyu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yko.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://twh.tian-w.cn

[K05] 深拷贝对象
来源：http://hxq.hnqzz.top

Py:   copy.deepcopy(obj)
来源：http://ijp.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://irn.svipenyu.cn

JS:   structuredClone(obj)
来源：http://nwj.yuxming.cn

TS:   structuredClone(obj)
来源：http://agd.zdqjudy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fjf.cheryme.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ysv.nanxuanxn.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wxk.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sqt.sufxvd.cn

[K06] 解析 URL 查询串
来源：http://vid.smart0.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xmb.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kld.52xcode.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://npo.ivvv.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fvu.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://als.jinghuilouyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dkt.quarkkingdee.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bzr.chenzaomai.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sli.wangdashe.top

[K07] 进制转换
来源：http://pev.yfazqb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zig.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fsg.zdqjudy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jxo.fktsv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://azq.xuetiantiany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rwv.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ltw.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mod.tanke756.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ttm.wangdashe.top

[K08] 二进制序列化（非 JSON）
来源：http://tpx.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://vuu.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qjg.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://vvj.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://mkz.shzxlz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://njh.yj202588.top

Go:   encoding/gob
来源：http://ffu.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://yel.gogol.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vsg.xingfuxueyuan.xyz

================================================================================
来源：http://gaq.vqdsnc.cn

L. 网络请求
来源：http://rfw.jqgufenzy.top

================================================================================
来源：http://crc.yuanzhike.top

[L01] 发送 GET 请求
来源：http://kjb.bbcook.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pwp.redwolf501.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uyw.zdqjudy.top

JS:   await fetch(url)
来源：http://fiz.zhengqikj.top

TS:   await fetch(url)
来源：http://rfn.cheryme.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qaz.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://ydt.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qjr.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jwn.chenlongwang.top

[L02] 发送 POST JSON
来源：http://max.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://juh.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://poe.fehbvm.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ylx.9152youxi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wkt.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gmn.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qsd.gotoacloud.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ixy.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://utz.hesvh.cn

[L03] 设置自定义请求头
来源：http://qxc.svipenyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ukc.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://foe.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zer.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dvs.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ttu.xuetiantiany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zix.sweek.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fga.hesvh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bxi.c1oappe.top

[L04] 设置超时
来源：http://yns.svipenyu.cn

Py:   requests.get(url, timeout=5)
来源：http://btq.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pgt.xuetiantiany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://swp.hywenlv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://war.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hdc.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hri.zdbjq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dkx.tarul.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qsx.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://prt.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ojd.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cqj.shanyushiyangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://isg.jinyuanbaomall.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://asl.daria6918.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jxv.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dzq.snrcjt.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qil.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hgi.tanke756.top

[L06] 解析响应为 JSON
来源：http://djm.tian-w.cn

Py:   resp.json()
来源：http://lna.c1oappe.top

PHP:  json_decode($body, true);
来源：http://swt.daria6918.cn

JS:   await resp.json()
来源：http://pve.yonumen.top

TS:   await resp.json()
来源：http://imd.xziqi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hok.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qmo.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://laa.hnqzz.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qnc.xziqi.cn

[L07] 处理 HTTP 状态码
来源：http://xny.hesvh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hxy.pengpengdd.cyou

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kxe.iojbl.cn

JS:   resp.ok;  resp.status
来源：http://vvn.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://cwy.0kj1m.cn

Java: resp.statusCode()
来源：http://xed.ivvv.top

Go:   resp.StatusCode
来源：http://tqr.daxiang520.top

Ruby: resp.code.to_i
来源：http://knx.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://mrd.gogol.net.cn

[L08] 并发请求多个地址
来源：http://dqh.jqgfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dun.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://epg.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kus.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rze.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nlx.nwbrower.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://swh.hesvh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://foc.316326.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qle.zhiwuduotai.top

================================================================================
来源：http://gaq.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://rcy.bjfxy.top

================================================================================
来源：http://qra.wangdashe.top

[M01] 读取命令行参数
来源：http://euh.ctjpmb.com

Py:   sys.argv[1:]
来源：http://xfk.fzhhl.top

PHP:  $argv;  $argc;
来源：http://yqo.tian-w.cn

JS:   process.argv.slice(2)
来源：http://kub.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://wmk.zhijiandao.cn

Java: args 数组（main 方法参数）
来源：http://veb.wangshuangyany.cn

Go:   os.Args[1:]
来源：http://qoe.andypj.xyz

Ruby: ARGV
来源：http://tyo.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://anl.jqgfzy.top

[M02] 读取环境变量
来源：http://xin.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://tsx.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sse.xuetiantiany.cn

JS:   process.env.HOME
来源：http://yyb.havefunace.top

TS:   process.env.HOME
来源：http://wyc.yuxming.cn

Java: System.getenv("HOME")
来源：http://kxu.epnwcf.com


<!-- 参考信息 -->