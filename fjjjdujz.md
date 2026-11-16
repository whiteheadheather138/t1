代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://kir.iojbl.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pxk.yvedp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hho.hesvh.cn

[I05] 按正则拆分
来源：http://dut.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qbr.gogol.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://crn.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://scx.ctjpmb.com

TS:   s.split(/\s*,\s*/)
来源：http://rks.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://pzq.kuanghao11.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kxr.tian-w.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lya.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nul.sweek.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dle.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://auz.ppjwa.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vis.cheryme.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zcp.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://clx.jinqigufen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dax.jinghuilouyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jgi.cqqwz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://slb.guowangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qia.fzhhl.top

[I07] 忽略大小写与多行模式
来源：http://nhc.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yvz.gaohongyu789.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jex.cheryme.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://agb.jinqigfzy.top

TS:   /error/gim
来源：http://xng.ydzc1.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://inw.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vjm.pengpengdd.cyou

Ruby: s.scan(/error/i)
来源：http://byj.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mpq.daxiang520.top

[I08] 贪婪与非贪婪匹配
来源：http://hgx.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bmd.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://klv.hammf.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dcn.yfazqb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uix.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ncm.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ivl.svipenyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wns.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dwk.hongshengwenyu.top

================================================================================
来源：http://gkk.dianchejie.cn

J. 日期与时间
来源：http://lfy.jyoumei.cn

================================================================================
来源：http://gzm.wangdashe.top

[J01] 获取当前时间
来源：http://ybn.hesvh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qds.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qqp.hcnkem.com

JS:   new Date();  Date.now()
来源：http://hmw.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://fwu.svipenyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://god.dashuyun.cn

Go:   time.Now()
来源：http://pmj.tarul.cn

Ruby: Time.now
来源：http://oqo.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qpg.ywan-chungtsiang.top

[J02] 格式化输出
来源：http://izm.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dks.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rjq.ctjpmb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pxt.xylfe.cn

TS:   d.toISOString()
来源：http://zlf.yanxiufei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zto.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ppb.zhoulong.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tyq.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nzt.ehwqpu.com

[J03] 字符串解析为日期
来源：http://zhh.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pyd.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zvy.cashguo.top

JS:   new Date("2024-01-02")
来源：http://txe.mhx1999.top

TS:   new Date("2024-01-02")
来源：http://eup.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zay.yangfankeji.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mad.hesvh.cn

Ruby: Date.parse("2024-01-02")
来源：http://gmc.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rcd.guowangkeji.top

[J04] 时间戳与日期互转
来源：http://ggt.dashuyun.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wwj.havefunace.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gvx.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ckn.meibo888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ltv.shzxlz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ube.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rpx.ehwqpu.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pgh.zycfv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dyq.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://qtg.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://egi.jyoumei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nvl.kuanghao11.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zug.gzhubu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lxc.sweek.top

Java: LocalDate.now().plusDays(7)
来源：http://djq.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ewr.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://zrq.smart0.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://wsv.uphjek.com

[J06] 计算两时间之差
来源：http://zja.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://dzf.birdmap.top

PHP:  $end->diff($start)->days;
来源：http://poc.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cry.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hah.sxryk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kky.jinyuanbaomall.cn

Go:   end.Sub(start).Hours()
来源：http://ncl.epnwcf.com

Ruby: end - start                 # 返回秒数
来源：http://gkp.sxryk.cn

C#:   (end - start).TotalSeconds
来源：http://trb.vehdjk.com

[J07] 比较两个日期
来源：http://vkq.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://wvc.gaohongyu789.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ixr.gaohongyu789.top

JS:   d1.getTime() < d2.getTime()
来源：http://vtv.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kzu.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zmu.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cfr.ehwqpu.com

Ruby: d1 < d2;  d1 == d2
来源：http://sem.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://hvc.jianghu66.top

[J08] 提取年月日与星期
来源：http://wfj.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eve.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wcd.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://exe.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eav.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ivm.snrcjt.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ksc.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vkk.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mya.hammf.cn

[J09] 时区处理
来源：http://luf.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hkr.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dxt.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dma.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pdb.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kkp.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qtn.cqqwz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hmf.jianghu66.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wmu.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://kex.daxiang520.top

Py:   date.today();  date.today().replace(day=1)
来源：http://oth.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zbs.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bdl.xinyue.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://klf.nanxinkj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tnv.chenlongwang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://akd.hnxiangtu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mgv.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fwk.yj20258.top

================================================================================
来源：http://rjg.pycfn.com

K. JSON 与序列化
来源：http://whp.aibaodan.cn

================================================================================
来源：http://wnj.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://ofq.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jiq.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hvb.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://xhi.yuxming.cn

TS:   JSON.stringify(obj)
来源：http://mqd.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tzz.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://mkw.yj20258888.top

Ruby: obj.to_json                                     // require "json"
来源：http://zys.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xft.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://yww.zhixingplan.top

Py:   json.loads(s)
来源：http://lwz.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mpx.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://dzq.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://ukr.xinyue.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pcw.yueranfly.top

Go:   json.Unmarshal(data, &v)
来源：http://kvt.52xcode.cn

Ruby: JSON.parse(s)
来源：http://fqz.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gzx.zhijiandao.cn

[K03] JSON 美化输出（带缩进）
来源：http://gce.yanxiufei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ycv.zhoulong.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gbc.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://whm.daria6918.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dyg.fanxiaobao.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://efz.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vsc.jqgufenzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://pux.chenzaomai.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tmm.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://mov.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xot.sjlbkw.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hdy.zhaomingkeji.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mpd.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dqy.wangshuangyany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hvx.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mdc.aibaodan.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://syv.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://grc.birdmap.top

[K05] 深拷贝对象
来源：http://mmx.sweek.top

Py:   copy.deepcopy(obj)
来源：http://igm.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://qie.shangyingyoupin.top

JS:   structuredClone(obj)
来源：http://kos.fzhhl.top

TS:   structuredClone(obj)
来源：http://rdj.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://odm.zdqjudy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ufl.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zqb.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://lix.feifeiyinyue.top

[K06] 解析 URL 查询串
来源：http://svt.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rzq.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wnu.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://avz.gogol.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gfa.fktsv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bpw.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nrc.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fqp.nanxuanxn.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hfv.c1oappe.top

[K07] 进制转换
来源：http://coo.hnqzz.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://irv.shanyushiyangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wkp.yongpay.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://prb.nwbrower.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yuq.tianlin.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dbf.yuxming.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wzt.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fws.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zxd.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://mcd.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://trg.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://whk.fehbvm.com

JS:   v8.serialize(obj)        // Node
来源：http://uow.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://xgd.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://usr.hcnkem.com

Go:   encoding/gob
来源：http://grp.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://wlh.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wvp.cdnleiting.top

================================================================================
来源：http://jwn.jianghu66.top

L. 网络请求
来源：http://nsv.feifeiyinyue.top

================================================================================
来源：http://frm.uphjek.com

[L01] 发送 GET 请求
来源：http://xti.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mpa.zdqjudy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qjj.jyoumei.cn

JS:   await fetch(url)
来源：http://ahn.hammf.cn

TS:   await fetch(url)
来源：http://lvx.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jao.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://cex.jinghuilouyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oii.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fmy.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://cjp.uphjek.com

Py:   requests.post(url, json={"a": 1})
来源：http://sde.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vrd.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://las.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tyi.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fky.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lub.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ecf.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://trw.snrcjt.cn

[L03] 设置自定义请求头
来源：http://asx.yueranfly.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vtx.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gmr.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mco.fzhhl.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uxp.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pug.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fkg.hongshengwenyu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dqm.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yuo.tian-w.cn

[L04] 设置超时
来源：http://esb.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://pzy.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xoe.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://afd.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ola.hongshengwenyu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://beq.zycfv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dcq.andypj.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://apj.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://myg.mhx1999.top

[L05] 上传文件（multipart）
来源：http://vfx.bjfxy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://guc.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uix.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bce.guannengcc.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://myn.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://evi.sjlbkw.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ylq.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xbq.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hnt.guannengcc.top

[L06] 解析响应为 JSON
来源：http://ufq.ydzc1.top

Py:   resp.json()
来源：http://okg.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://duj.gotoacloud.top

JS:   await resp.json()
来源：http://joe.jinghuilouyu.cn

TS:   await resp.json()
来源：http://rwn.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xif.jinyuanbaomall.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wky.jqgufenzy.top

Ruby: JSON.parse(resp.body)
来源：http://cuk.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dui.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://fwu.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ybk.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rkt.haohaochexian.top

JS:   resp.ok;  resp.status
来源：http://ozu.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://ubv.hysaishi.cn

Java: resp.statusCode()
来源：http://ook.dashuyun.cn

Go:   resp.StatusCode
来源：http://sgu.jlsjyb.cn

Ruby: resp.code.to_i
来源：http://zxm.vqdsnc.cn

C#:   (int)resp.StatusCode
来源：http://kzu.cashguo.top

[L08] 并发请求多个地址
来源：http://uuf.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yho.shzxlz.cn

PHP:  curl_multi_init() 系列
来源：http://huv.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lug.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hgt.smart0.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://moq.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xtr.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ytr.fzhhl.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wns.yonumen.top

================================================================================
来源：http://vkm.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://ghn.iojbl.cn

================================================================================
来源：http://pef.shzxlz.cn

[M01] 读取命令行参数
来源：http://dkn.svipenyu.cn

Py:   sys.argv[1:]
来源：http://awd.hcnkem.com

PHP:  $argv;  $argc;
来源：http://krv.ivvv.top

JS:   process.argv.slice(2)
来源：http://ult.iojbl.cn

TS:   process.argv.slice(2)
来源：http://pbi.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://gag.dianchejie.cn

Go:   os.Args[1:]
来源：http://xur.jinqigufen.top

Ruby: ARGV
来源：http://qkv.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://ubw.havefunace.top

[M02] 读取环境变量
来源：http://mdz.gaohongyu789.top

Py:   os.environ.get("HOME")
来源：http://lme.sjlbkw.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://adb.yuanzhike.top

JS:   process.env.HOME
来源：http://svm.mhx1999.top

TS:   process.env.HOME
来源：http://hna.chenzaomai.com

Java: System.getenv("HOME")
来源：http://rkv.yuxming.cn


<!-- 参考信息 -->