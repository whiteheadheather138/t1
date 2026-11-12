代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://wng.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jtv.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fkl.meibo888.top

[I05] 按正则拆分
来源：http://zjz.gogol.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vis.zhengqikj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yag.birdmap.top

JS:   s.split(/\s*,\s*/)
来源：http://hyt.kuanghao11.cn

TS:   s.split(/\s*,\s*/)
来源：http://qgd.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://qdv.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dix.9152youxi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lkm.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://svx.aibaodan.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zmx.cucudq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ywh.epnwcf.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gds.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oyy.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://msq.hnqzz.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ueu.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jrr.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xkw.tarul.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://crv.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://cgp.zhaomingkeji.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zbz.xylfe.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tvl.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eik.pycfn.com

TS:   /error/gim
来源：http://evr.hnqzz.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gka.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nex.zhijiandao.cn

Ruby: s.scan(/error/i)
来源：http://ysn.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qfi.ivvv.top

[I08] 贪婪与非贪婪匹配
来源：http://xzd.yuxming.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fon.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mbo.gogol.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ppp.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qvr.yfazqb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://prg.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tdh.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gfp.dashuyun.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oad.sxryk.cn

================================================================================
来源：http://qiw.zycfv.cn

J. 日期与时间
来源：http://jmi.zhongyouzk.top

================================================================================
来源：http://cxb.guowangkeji.top

[J01] 获取当前时间
来源：http://yid.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kuq.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://low.hnqzz.top

JS:   new Date();  Date.now()
来源：http://rzy.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://nuf.quarkkingdee.top

Java: LocalDateTime.now();  Instant.now()
来源：http://miz.hammf.cn

Go:   time.Now()
来源：http://zae.shanyushiyangkeji.top

Ruby: Time.now
来源：http://tjs.cashguo.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ise.andypj.xyz

[J02] 格式化输出
来源：http://fau.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://edf.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qcq.ivvv.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xsp.fehbvm.com

TS:   d.toISOString()
来源：http://sbr.smart0.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hix.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://diq.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wlg.feifeiyinyue.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ldc.hammf.cn

[J03] 字符串解析为日期
来源：http://eow.tanke756.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gil.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kbw.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://dpg.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://fur.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://glw.feifeiyinyue.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eaj.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://vxe.wangdashe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xxk.hammf.cn

[J04] 时间戳与日期互转
来源：http://psm.birdmap.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oon.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uyt.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xcr.sjlbkw.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mvc.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ifn.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uvp.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gja.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oax.ywan-chungtsiang.top

[J05] 时间加减（加 7 天）
来源：http://tun.jlsjyb.cn

Py:   now + timedelta(days=7)
来源：http://uqb.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://psd.sysykeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rjs.shanyushiyangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ogk.jianghu66.top

Java: LocalDate.now().plusDays(7)
来源：http://pnc.yueranfly.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jaz.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://suf.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rvr.kuanghao11.cn

[J06] 计算两时间之差
来源：http://vsb.yj202588.top

Py:   (end - start).total_seconds()
来源：http://bjt.jqgfzy.top

PHP:  $end->diff($start)->days;
来源：http://wsf.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://czi.xingfuxueyuan.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://byd.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://sgl.vehdjk.com

Go:   end.Sub(start).Hours()
来源：http://mzd.zycfv.cn

Ruby: end - start                 # 返回秒数
来源：http://qjf.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://mhb.cdnleiting.top

[J07] 比较两个日期
来源：http://dnx.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://oxv.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nxt.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hyz.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://lnt.tarul.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lmw.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xxi.hysaishi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zqb.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://sno.jyoumei.cn

[J08] 提取年月日与星期
来源：http://zzp.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://irs.hnxiangtu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zmr.feifeiyinyue.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zgj.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wxw.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jcf.ydjk.org.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rqa.shzxlz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ohn.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lvl.gotoacloud.top

[J09] 时区处理
来源：http://uoi.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lvp.pengpengdd.cyou

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sbi.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cdd.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vxy.yfazqb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bta.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fag.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://cvx.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gfa.tanke756.top

[J10] 取今天 / 本月第一天
来源：http://tym.cashguo.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gcg.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rjh.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://phs.zycfv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nxk.tanke756.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dvj.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://auw.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mcv.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nys.zycfv.cn

================================================================================
来源：http://ugh.xuetiantiany.cn

K. JSON 与序列化
来源：http://qyc.xinyue.icu

================================================================================
来源：http://kif.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://ukh.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://szy.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dfo.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://axo.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://njp.kuanghao11.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jzq.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://utn.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://cin.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dmg.tarul.cn

[K02] JSON 字符串转对象
来源：http://suw.sufxvd.cn

Py:   json.loads(s)
来源：http://uoc.guowangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rsz.havefunace.top

JS:   JSON.parse(s)
来源：http://pfp.haohaochexian.top

TS:   JSON.parse(s)
来源：http://gdd.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ygl.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://adq.xziqi.cn

Ruby: JSON.parse(s)
来源：http://ijj.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lwa.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://nah.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fex.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://weg.smart0.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://xvj.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ysv.yueranfly.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cxo.redwolf501.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zmk.chenjidiqi.icu

Ruby: JSON.pretty_generate(obj)
来源：http://zkm.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hpv.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://qdx.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://flg.tianlin.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lxw.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iyi.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xdt.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gbp.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jrh.jqgfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://toc.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yml.hcnkem.com

[K05] 深拷贝对象
来源：http://yzo.hesvh.cn

Py:   copy.deepcopy(obj)
来源：http://sbr.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://uhs.haohaochexian.top

JS:   structuredClone(obj)
来源：http://txh.mhx1999.top

TS:   structuredClone(obj)
来源：http://wed.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lof.yj202588.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jtx.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zow.sysykeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bka.dianchejie.cn

[K06] 解析 URL 查询串
来源：http://oxc.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cnc.bjfxy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cxy.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tzu.mhx1999.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qxm.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mdg.9152youxi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://aco.xylfe.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xuv.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tjh.zycfv.cn

[K07] 进制转换
来源：http://rqk.tian-w.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hrc.zdbjq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gel.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://caf.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kjk.bjfxy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hlb.fehbvm.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://err.hcnkem.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kkm.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pgj.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://gew.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://nqj.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lek.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://vfs.chenzaomai.com

TS:   v8.serialize(obj)        // Node
来源：http://cgt.yvedp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zbh.yonumen.top

Go:   encoding/gob
来源：http://vjs.gogol.net.cn

Ruby: Marshal.dump(obj)
来源：http://mga.gogol.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cga.cdnleiting.top

================================================================================
来源：http://hao.cucudq.cn

L. 网络请求
来源：http://ill.pengpengdd.cyou

================================================================================
来源：http://des.c1oappe.top

[L01] 发送 GET 请求
来源：http://jpy.mhx1999.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://put.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bis.hnxiangtu.top

JS:   await fetch(url)
来源：http://ydu.quarkkingdee.top

TS:   await fetch(url)
来源：http://sak.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vfa.tianlin.xyz

Go:   resp, err := http.Get(url)
来源：http://skg.0kj1m.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gdx.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://efn.yuxming.cn

[L02] 发送 POST JSON
来源：http://xhh.daxiang520.top

Py:   requests.post(url, json={"a": 1})
来源：http://qef.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qnk.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lgk.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nmj.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tsm.nanxuanxn.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://juf.hammf.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xed.xylfe.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://afn.havefunace.top

[L03] 设置自定义请求头
来源：http://rxv.birdmap.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://huf.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aqq.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ral.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://imn.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fhu.shuidangran.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nci.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://opt.yuanzhike.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ija.ywan-chungtsiang.top

[L04] 设置超时
来源：http://gxl.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://xgm.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://frr.cdnleiting.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xmq.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sqe.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ndm.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://svr.tianlin.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://soz.havefunace.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ijv.daxiang520.top

[L05] 上传文件（multipart）
来源：http://pqg.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yse.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yyx.yj20258.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vfb.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bht.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hgt.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://obl.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jhu.aibaodan.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hdr.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://rov.jianghu66.top

Py:   resp.json()
来源：http://kvo.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://pbx.shzxlz.cn

JS:   await resp.json()
来源：http://sne.sjlbkw.cn

TS:   await resp.json()
来源：http://eup.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tji.tianlin.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jby.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://pov.pengpengdd.cyou

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ygl.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://ucz.jiagoushi.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aiz.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lug.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://dze.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://xrd.mhx1999.top

Java: resp.statusCode()
来源：http://trf.fzhhl.top

Go:   resp.StatusCode
来源：http://mvo.zhixingplan.top

Ruby: resp.code.to_i
来源：http://zbj.nwbrower.top

C#:   (int)resp.StatusCode
来源：http://kkr.gzhubu.top

[L08] 并发请求多个地址
来源：http://obw.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tyk.zhixingplan.top

PHP:  curl_multi_init() 系列
来源：http://qic.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lln.haohaochexian.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bgh.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zjq.hongshengwenyu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://krb.zhixingplan.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zul.dianchejie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nxh.fengsongda.top

================================================================================
来源：http://hiu.tian-w.cn

M. 命令行 / 进程 / 环境
来源：http://jaa.zdbjq.cn

================================================================================
来源：http://qec.yj202588.top

[M01] 读取命令行参数
来源：http://swm.uphjek.com

Py:   sys.argv[1:]
来源：http://xim.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://dgo.zhaomingkeji.xyz

JS:   process.argv.slice(2)
来源：http://pjq.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://ayw.316326.xyz

Java: args 数组（main 方法参数）
来源：http://hti.zhoulong.xyz

Go:   os.Args[1:]
来源：http://dgs.guowangkeji.top

Ruby: ARGV
来源：http://oeu.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://zgn.zycfv.cn

[M02] 读取环境变量
来源：http://iqq.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://dxx.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hcs.cucudq.cn

JS:   process.env.HOME
来源：http://xrz.cqqwz.cn

TS:   process.env.HOME
来源：http://bxn.shanyushiyangtech.top

Java: System.getenv("HOME")
来源：http://aqs.epnwcf.com


<!-- 参考信息 -->