代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yuy.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jjw.tian-w.cn

[I04] 正则替换
来源：http://iin.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://iym.sysykeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rpj.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://baf.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://rse.chenlongwang.top

Java: s.replaceAll("\\d+", "#")
来源：http://wpd.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ozs.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fzy.ppjwa.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lyj.zhoulong.xyz

[I05] 按正则拆分
来源：http://ldo.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hpn.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vxv.daria6918.cn

JS:   s.split(/\s*,\s*/)
来源：http://yxd.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://rlc.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://mkz.havefunace.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wri.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://wdu.hnxiangtu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oks.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dhc.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ohs.quarkkingdee.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bnw.yonumen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pga.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wuq.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mlp.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ped.uphjek.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jxv.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pwv.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://ukg.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rgd.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yfk.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kig.redwolf501.top

TS:   /error/gim
来源：http://tdi.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vmg.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mpj.yfazqb.com

Ruby: s.scan(/error/i)
来源：http://ogy.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fto.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://goy.daxiang520.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wpp.wangshuangyany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ehw.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://puu.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://flc.jianghu66.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tcr.yuxming.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mhp.zhongyouzk.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gjl.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pdz.mhx1999.top

================================================================================
来源：http://kuf.gzhubu.top

J. 日期与时间
来源：http://hgy.shanyushiyangkeji.top

================================================================================
来源：http://hmp.redwolf501.top

[J01] 获取当前时间
来源：http://xbp.yj20258.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://sqr.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pon.jinyuanbaomall.cn

JS:   new Date();  Date.now()
来源：http://gff.zhijiandao.cn

TS:   new Date();  Date.now()
来源：http://suu.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hzd.jianghu66.top

Go:   time.Now()
来源：http://ifk.meibo888.top

Ruby: Time.now
来源：http://fyy.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kph.iojbl.cn

[J02] 格式化输出
来源：http://ouf.yuanzhike.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eia.ydjk.org.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yvc.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dyk.chenzaomai.com

TS:   d.toISOString()
来源：http://hvj.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qow.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mky.hnxiangtu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pyj.yvedp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yzm.sxryk.cn

[J03] 字符串解析为日期
来源：http://pyv.chenjidiqi.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iey.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hym.hcnkem.com

JS:   new Date("2024-01-02")
来源：http://ste.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://tse.iojbl.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bxq.wangshuangyany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zzt.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://cun.yuanzhike.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cej.birdmap.top

[J04] 时间戳与日期互转
来源：http://ipz.yvedp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://maf.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xpr.9152youxi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xyk.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://urx.jqgfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gae.jqgfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nxh.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://amr.jinyuanbaomall.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bba.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://jpe.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://iid.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hcz.ydjk.org.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ndk.iojbl.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mlw.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://igz.wangdashe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wog.cqqwz.cn

Ruby: Time.now + 7 * 86400
来源：http://qvl.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://coh.hnqzz.top

[J06] 计算两时间之差
来源：http://usq.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://txd.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://pbn.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://riu.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://phl.ehwqpu.com

Java: Duration.between(start, end).toSeconds()
来源：http://wgc.cucudq.cn

Go:   end.Sub(start).Hours()
来源：http://nrp.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://erd.cucudq.cn

C#:   (end - start).TotalSeconds
来源：http://kzs.xziqi.cn

[J07] 比较两个日期
来源：http://lez.ctjpmb.com

Py:   d1 < d2;  d1 == d2
来源：http://ptv.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kgl.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://atp.jinghuilouyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://miz.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uui.hongshengwenyu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hrr.feifeiyinyue.top

Ruby: d1 < d2;  d1 == d2
来源：http://quv.aizwys.cn

C#:   d1 < d2;  d1 == d2
来源：http://qbn.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://guw.tianlin.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://plm.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zmx.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kmq.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vga.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://upa.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zlf.zhengqikj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://haa.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mff.jinyuanbaomall.cn

[J09] 时区处理
来源：http://edb.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ndw.yangfankeji.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nsi.dianchejie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://crn.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dyk.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iim.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ika.haohaochexian.top

Ruby: Time.now.getlocal("+08:00")
来源：http://amf.jianghu66.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sxn.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://hxz.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xis.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uxj.tarul.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dmo.cashguo.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wxy.hysaishi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jqf.epnwcf.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vle.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pyn.hnqzz.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vra.sufxvd.cn

================================================================================
来源：http://fnj.tianlin.xyz

K. JSON 与序列化
来源：http://qqe.316326.xyz

================================================================================
来源：http://tks.hnqzz.top

[K01] 对象转 JSON 字符串
来源：http://vnu.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gnf.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kyt.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://jgn.birdmap.top

TS:   JSON.stringify(obj)
来源：http://otv.ydzc1.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://met.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://wtr.fengsongda.top

Ruby: obj.to_json                                     // require "json"
来源：http://qrv.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://sge.sweek.top

[K02] JSON 字符串转对象
来源：http://dhx.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://soj.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yxk.fanxiaobao.xyz

JS:   JSON.parse(s)
来源：http://ypz.cqqwz.cn

TS:   JSON.parse(s)
来源：http://rtl.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://saj.hammf.cn

Go:   json.Unmarshal(data, &v)
来源：http://wzl.hysaishi.cn

Ruby: JSON.parse(s)
来源：http://grq.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xzx.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://okr.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://msg.dianchejie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kqk.hysaishi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dhe.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ult.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ret.jyoumei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rnz.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://qoy.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oru.xinyue.icu

[K04] 读取 JSON 文件
来源：http://him.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wmj.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://irx.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pxy.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tcf.xingfuxueyuan.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wuk.yueranfly.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zbe.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://ovj.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oed.hcnkem.com

[K05] 深拷贝对象
来源：http://ttm.jqgufenzy.top

Py:   copy.deepcopy(obj)
来源：http://fie.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://iul.meibo888.top

JS:   structuredClone(obj)
来源：http://tzb.shuidangran.top

TS:   structuredClone(obj)
来源：http://usw.xylfe.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ziz.xingfuxueyuan.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tux.hywenlv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://syr.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zot.tarul.cn

[K06] 解析 URL 查询串
来源：http://rcx.zhongyouzk.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cfk.guowangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://swf.fzhhl.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://etg.bjfxy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xyr.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oel.ydzc1.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://grv.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qpo.ehwqpu.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kkb.jlsjyb.cn

[K07] 进制转换
来源：http://cws.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cye.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pgt.shanyushiyangtech.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bxt.dashuyun.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://aac.gaohongyu789.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lar.tianlin.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fai.jqgfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pnw.feifeiyinyue.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hzn.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://boy.316326.xyz

Py:   pickle.dumps(obj)
来源：http://dur.c1oappe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zww.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://vwe.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://fyf.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rew.hcnkem.com

Go:   encoding/gob
来源：http://jxh.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://vts.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dbf.zhongyouzk.top

================================================================================
来源：http://nwx.tian-w.cn

L. 网络请求
来源：http://aiu.quarkkingdee.top

================================================================================
来源：http://ple.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://pau.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xiv.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bvk.nanxinkj.top

JS:   await fetch(url)
来源：http://pgy.0kj1m.cn

TS:   await fetch(url)
来源：http://znx.nwbrower.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://emd.zycfv.cn

Go:   resp, err := http.Get(url)
来源：http://efd.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://dbn.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://irp.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://xce.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://kji.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fsv.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gvn.gogol.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iiy.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bca.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wcl.xingfuxueyuan.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wxb.yuxming.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gdv.zhengqikj.top

[L03] 设置自定义请求头
来源：http://awq.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jrh.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ygy.iojbl.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://njn.jinyuanbaomall.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kcz.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mrj.hesvh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://anr.fzhhl.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rng.guowangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fmg.cucudq.cn

[L04] 设置超时
来源：http://vxs.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://glg.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qrw.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jsj.yj202588.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://miz.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://res.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://krh.xuanzx.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rvi.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tiz.ywan-chungtsiang.top

[L05] 上传文件（multipart）
来源：http://kqz.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dcu.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://twv.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bfc.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kpe.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://saf.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lsn.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fqd.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fus.zdbjq.cn

[L06] 解析响应为 JSON
来源：http://ykx.hnqzz.top

Py:   resp.json()
来源：http://szo.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://qgk.guowangkeji.top

JS:   await resp.json()
来源：http://fou.wangdashe.top

TS:   await resp.json()
来源：http://tof.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dew.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fqe.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://uee.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wxq.hongshengwenyu.top

[L07] 处理 HTTP 状态码
来源：http://cim.birdmap.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mig.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zic.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://nqv.0kj1m.cn

TS:   resp.ok;  resp.status
来源：http://mhn.sweek.top

Java: resp.statusCode()
来源：http://rht.wangshuangyany.cn

Go:   resp.StatusCode
来源：http://mfb.bbcook.cn

Ruby: resp.code.to_i
来源：http://hou.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://okd.meibo888.top

[L08] 并发请求多个地址
来源：http://bcz.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jsc.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://rio.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://agy.zdqjudy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ocq.zhixingplan.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jmx.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ynn.mhx1999.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nal.ctjpmb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dgv.feifeiyinyue.top

================================================================================
来源：http://uch.zdbjq.cn

M. 命令行 / 进程 / 环境
来源：http://bid.bbcook.cn

================================================================================
来源：http://nqe.jinqigufen.top

[M01] 读取命令行参数
来源：http://mlq.zdqjudy.top

Py:   sys.argv[1:]
来源：http://lix.ydjk.org.cn

PHP:  $argv;  $argc;
来源：http://gdg.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://nmm.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://vgw.yuanzhike.top

Java: args 数组（main 方法参数）
来源：http://qdl.chenlongwang.top

Go:   os.Args[1:]
来源：http://xph.zhoulong.xyz


<!-- 参考信息 -->