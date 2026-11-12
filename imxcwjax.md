代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qbq.hongshengwenyu.top

[I03] 提取捕获分组
来源：http://ena.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eqz.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hxk.nanxuanxn.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wjc.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://epp.hnxiangtu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lzp.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ojy.shanyushiyangtech.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hlt.dashuyun.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://soq.nwbrower.top

[I04] 正则替换
来源：http://pml.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qyu.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uby.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ngr.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://uok.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://agi.ybcxt.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gpw.cashguo.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dfb.hongshengwenyu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nub.gaohongyu789.top

[I05] 按正则拆分
来源：http://ozl.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jac.dianchejie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wyh.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://shn.fanxiaobao.xyz

TS:   s.split(/\s*,\s*/)
来源：http://vbg.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://bvx.hcnkem.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rec.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://eqf.guowangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vmu.chenzaomai.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blr.ehwqpu.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fsi.fanxiaobao.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ame.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tdm.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rvt.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ywu.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yte.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ddn.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cxh.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://hnx.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wba.yonumen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://krf.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yus.zdqjudy.top

TS:   /error/gim
来源：http://otf.shanyushiyangtech.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ipe.yuanzhike.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hai.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://pog.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hdh.ivvv.top

[I08] 贪婪与非贪婪匹配
来源：http://rse.yonumen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oks.yanxiufei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gtf.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ihy.gotoacloud.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kul.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://his.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aml.ppjwa.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://omk.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jzf.gzhubu.top

================================================================================
来源：http://evw.gogol.net.cn

J. 日期与时间
来源：http://fsa.feifeiyinyue.top

================================================================================
来源：http://cbq.svipenyu.cn

[J01] 获取当前时间
来源：http://wzb.haohaochexian.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ged.yfazqb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nek.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://gnd.smart0.xyz

TS:   new Date();  Date.now()
来源：http://sgz.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://klt.daria6918.cn

Go:   time.Now()
来源：http://uat.ivvv.top

Ruby: Time.now
来源：http://ocz.tianlin.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nda.yuxming.cn

[J02] 格式化输出
来源：http://woh.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lau.chenlongwang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hts.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xtc.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://vch.jinqigfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uvy.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bfh.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ppj.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lcg.xingfuxueyuan.xyz

[J03] 字符串解析为日期
来源：http://msn.shzxlz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://swd.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pov.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://qoc.hongshengwenyu.top

TS:   new Date("2024-01-02")
来源：http://ypx.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xld.haohaochexian.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hss.ydjk.org.cn

Ruby: Date.parse("2024-01-02")
来源：http://exx.shanyushiyangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rud.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://ywl.pengpengdd.cyou

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dlc.cqqwz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jyn.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://myf.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mfe.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gke.iojbl.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cxu.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sfx.hcnkem.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qsv.jinqigfzy.top

[J05] 时间加减（加 7 天）
来源：http://pwa.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://ttd.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ryj.sufxvd.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://evp.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rnm.hnqzz.top

Java: LocalDate.now().plusDays(7)
来源：http://ggy.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rak.ppjwa.cn

Ruby: Time.now + 7 * 86400
来源：http://oeh.jqgufenzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://lzf.redwolf501.top

[J06] 计算两时间之差
来源：http://ood.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://jvn.ehwqpu.com

PHP:  $end->diff($start)->days;
来源：http://msc.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://awt.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yci.redwolf501.top

Java: Duration.between(start, end).toSeconds()
来源：http://jix.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://fxg.shanyushiyangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://atu.bjfxy.top

C#:   (end - start).TotalSeconds
来源：http://pmh.bbcook.cn

[J07] 比较两个日期
来源：http://lbf.hnqzz.top

Py:   d1 < d2;  d1 == d2
来源：http://gue.guowangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kae.yuxming.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ojm.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://qty.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uth.ybcxt.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pny.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cqx.shangyingyoupin.top

C#:   d1 < d2;  d1 == d2
来源：http://win.yuxming.cn

[J08] 提取年月日与星期
来源：http://olp.iojbl.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wht.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oem.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pdh.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yqi.redwolf501.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mri.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ujt.cheryme.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xlz.jyoumei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://riu.haohaochexian.top

[J09] 时区处理
来源：http://fmx.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jvd.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://scr.sysykeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yqw.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://isg.9152youxi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oih.yj20258888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hsk.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://amq.meibo888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blb.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://wnq.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hcl.iojbl.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rpn.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://brh.gaohongyu789.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jrb.guannengcc.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zbm.redwolf501.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fmj.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sev.smart0.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jsa.uphjek.com

================================================================================
来源：http://lys.sysykeji.top

K. JSON 与序列化
来源：http://snq.yangfankeji.com

================================================================================
来源：http://ggh.chenjidiqi.icu

[K01] 对象转 JSON 字符串
来源：http://rae.iojbl.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://epf.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jpr.hnxiangtu.top

JS:   JSON.stringify(obj)
来源：http://duh.nanxinkj.top

TS:   JSON.stringify(obj)
来源：http://vcw.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kzk.ybcxt.top

Go:   json.Marshal(obj)
来源：http://wyz.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://oaw.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tyz.vehdjk.com

[K02] JSON 字符串转对象
来源：http://hol.ydjk.org.cn

Py:   json.loads(s)
来源：http://vbz.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vud.ywan-chungtsiang.top

JS:   JSON.parse(s)
来源：http://zku.dashuyun.cn

TS:   JSON.parse(s)
来源：http://vrs.yueranfly.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://con.fzhhl.top

Go:   json.Unmarshal(data, &v)
来源：http://zgk.tanke756.top

Ruby: JSON.parse(s)
来源：http://ynu.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mwi.xylfe.cn

[K03] JSON 美化输出（带缩进）
来源：http://jvd.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lzo.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qav.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kri.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kce.ehwqpu.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iiw.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rmv.yj20258.top

Ruby: JSON.pretty_generate(obj)
来源：http://hje.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ofw.iojbl.cn

[K04] 读取 JSON 文件
来源：http://qkf.daria6918.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://afr.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jqs.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rie.yanxiufei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jig.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://stk.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nbw.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://jsk.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nrb.aibaodan.cn

[K05] 深拷贝对象
来源：http://amk.smart0.xyz

Py:   copy.deepcopy(obj)
来源：http://lce.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://osa.jinqigfzy.top

JS:   structuredClone(obj)
来源：http://ihk.tanke756.top

TS:   structuredClone(obj)
来源：http://vuw.jiagoushi.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xoq.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kyd.uphjek.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://meq.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jnd.shanyushiyangtech.top

[K06] 解析 URL 查询串
来源：http://gil.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zku.gaohongyu789.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://itw.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aqh.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://isy.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yln.bbcook.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ymh.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://epg.cashguo.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xga.nwbrower.top

[K07] 进制转换
来源：http://ovi.hywenlv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iap.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lcf.sufxvd.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xuj.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pnk.bjfxy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xfe.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xps.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mku.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kbm.sufxvd.cn

[K08] 二进制序列化（非 JSON）
来源：http://rkg.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://yvu.yj20258.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ekm.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://xdm.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://deu.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eue.sxryk.cn

Go:   encoding/gob
来源：http://tlp.ppjwa.cn

Ruby: Marshal.dump(obj)
来源：http://hvu.xylfe.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fsx.iojbl.cn

================================================================================
来源：http://qvj.yuxming.cn

L. 网络请求
来源：http://vev.gaohongyu789.top

================================================================================
来源：http://ysj.tanke756.top

[L01] 发送 GET 请求
来源：http://mnr.nwbrower.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mov.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ybo.zhoulong.xyz

JS:   await fetch(url)
来源：http://ijb.smart0.xyz

TS:   await fetch(url)
来源：http://qac.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eym.xuetiantiany.cn

Go:   resp, err := http.Get(url)
来源：http://mpz.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bjs.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xkr.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://yeg.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://war.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://svs.yj202588.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yne.hcnkem.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mdp.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jus.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iij.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dqf.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xqm.pycfn.com

[L03] 设置自定义请求头
来源：http://ppz.ywan-chungtsiang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ekq.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pum.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rys.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oqm.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pfc.xziqi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://npi.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vux.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tzx.hesvh.cn

[L04] 设置超时
来源：http://jtd.vqdsnc.cn

Py:   requests.get(url, timeout=5)
来源：http://gtu.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dee.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ahx.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hix.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ght.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pwm.zycfv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xuw.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qup.epnwcf.com

[L05] 上传文件（multipart）
来源：http://lsq.jianghu66.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ywx.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zyh.tarul.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fru.hywenlv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zlm.zhengqikj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ice.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ubw.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pre.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kfv.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://pvg.yongpay.top

Py:   resp.json()
来源：http://cst.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://lnz.c1oappe.top

JS:   await resp.json()
来源：http://pto.ctjpmb.com

TS:   await resp.json()
来源：http://qlm.aibaodan.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mxc.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://enb.316326.xyz

Ruby: JSON.parse(resp.body)
来源：http://lvz.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ibu.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://fun.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xmm.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jez.hcnkem.com

JS:   resp.ok;  resp.status
来源：http://imj.gzhubu.top

TS:   resp.ok;  resp.status
来源：http://elx.vehdjk.com

Java: resp.statusCode()
来源：http://ugc.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://uat.chenlongwang.top

Ruby: resp.code.to_i
来源：http://pmf.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://lge.aizwys.cn

[L08] 并发请求多个地址
来源：http://ynu.bbcook.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pty.snrcjt.cn

PHP:  curl_multi_init() 系列
来源：http://wyv.cqqwz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dvi.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nlp.zhoulong.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kjp.pengpengdd.cyou

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qxe.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zci.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kfw.xingfuxueyuan.xyz

================================================================================
来源：http://lxw.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://wkm.cucudq.cn


<!-- 参考信息 -->