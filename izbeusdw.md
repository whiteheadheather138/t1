代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://afu.vqdsnc.cn

[I03] 提取捕获分组
来源：http://ezg.zhoulong.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tmc.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aby.yj20258888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://loh.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vks.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gpg.dianchejie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kfz.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pyz.fehbvm.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pzs.yj202588.top

[I04] 正则替换
来源：http://yxv.feifeiyinyue.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ffm.jinyuanbaomall.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lzu.meibo888.top

JS:   s.replace(/\d+/g, "#")
来源：http://hun.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qtm.zdbjq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pag.tarul.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://iii.zhixingplan.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uhf.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mfe.jinyuanbaomall.cn

[I05] 按正则拆分
来源：http://opj.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wba.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tyj.ctjpmb.com

JS:   s.split(/\s*,\s*/)
来源：http://szy.jqgfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://fgo.iojbl.cn

Java: s.split("\\s*,\\s*")
来源：http://nxe.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hwj.ehwqpu.com

Ruby: s.split(/\s*,\s*/)
来源：http://bdx.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gfe.yfazqb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ilb.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zez.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vmu.xuanzx.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iws.nwbrower.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mbz.shangyingyoupin.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ulj.cucudq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ard.feifeiyinyue.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ggm.xinyue.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sln.xziqi.cn

[I07] 忽略大小写与多行模式
来源：http://kzw.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://smj.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ipj.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://skh.cdnleiting.top

TS:   /error/gim
来源：http://owd.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://crw.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mwo.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://xji.haohaochexian.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kvg.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://stx.daria6918.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dpj.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pxx.sxryk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xmz.cashguo.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yer.ctjpmb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://gye.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qyf.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jcs.zhijiandao.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bmp.hesvh.cn

================================================================================
来源：http://rpk.epnwcf.com

J. 日期与时间
来源：http://xrd.jinqigufen.top

================================================================================
来源：http://ugs.jinqigfzy.top

[J01] 获取当前时间
来源：http://yfu.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hma.nwbrower.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://udy.fengsongda.top

JS:   new Date();  Date.now()
来源：http://hmk.quarkkingdee.top

TS:   new Date();  Date.now()
来源：http://jti.xingfuxueyuan.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://xaa.wangshuangyany.cn

Go:   time.Now()
来源：http://njk.jinqigufen.top

Ruby: Time.now
来源：http://dzh.shanyushiyangtech.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://afi.yvedp.cn

[J02] 格式化输出
来源：http://oah.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cqu.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xyz.jyoumei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lta.sufxvd.cn

TS:   d.toISOString()
来源：http://vej.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cnb.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vyy.gzhubu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zez.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tze.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://agd.gaohongyu789.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ycu.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://shc.yongpay.top

JS:   new Date("2024-01-02")
来源：http://usi.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://khz.yj202588.top

Java: LocalDate.parse("2024-01-02")
来源：http://ckm.xziqi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xzj.aizwys.cn

Ruby: Date.parse("2024-01-02")
来源：http://dzy.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pxz.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://idb.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://szk.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xba.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zuv.meibo888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yhr.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lfp.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://luh.hywenlv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hfq.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oxi.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://dia.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://xwh.ppjwa.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zkf.gzhubu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jvp.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gbi.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://ycn.tianlin.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://spu.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://atg.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://eyg.svipenyu.cn

[J06] 计算两时间之差
来源：http://ndn.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://kof.haohaochexian.top

PHP:  $end->diff($start)->days;
来源：http://qnn.hysaishi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vfh.ctjpmb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dsg.ywan-chungtsiang.top

Java: Duration.between(start, end).toSeconds()
来源：http://bdm.cqqwz.cn

Go:   end.Sub(start).Hours()
来源：http://ymt.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://qgk.ppjwa.cn

C#:   (end - start).TotalSeconds
来源：http://eaw.nanxuanxn.top

[J07] 比较两个日期
来源：http://ayy.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://uor.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://smf.316326.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://ydq.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://rsf.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rgj.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pla.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://opf.gotoacloud.top

C#:   d1 < d2;  d1 == d2
来源：http://wme.dashuyun.cn

[J08] 提取年月日与星期
来源：http://uxf.tarul.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nae.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xcs.yongpay.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jyp.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ebq.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nay.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://abu.jlsjyb.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fpz.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nxv.shzxlz.cn

[J09] 时区处理
来源：http://jkm.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yns.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://umv.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yjx.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bos.yfazqb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kbh.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hit.cqqwz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://coh.yj202588.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sjp.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://fzv.yueranfly.top

Py:   date.today();  date.today().replace(day=1)
来源：http://znb.ybcxt.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aib.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mzl.fktsv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bcp.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rep.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tpa.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lyt.jyoumei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zag.chenlongwang.top

================================================================================
来源：http://hau.tanke756.top

K. JSON 与序列化
来源：http://tes.yangfankeji.com

================================================================================
来源：http://fuq.xylfe.cn

[K01] 对象转 JSON 字符串
来源：http://zcq.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://spm.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://avf.ivvv.top

JS:   JSON.stringify(obj)
来源：http://tes.ivvv.top

TS:   JSON.stringify(obj)
来源：http://ulb.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kkj.316326.xyz

Go:   json.Marshal(obj)
来源：http://kyb.c1oappe.top

Ruby: obj.to_json                                     // require "json"
来源：http://tko.jqgfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ffo.andypj.xyz

[K02] JSON 字符串转对象
来源：http://jxv.pengpengdd.cyou

Py:   json.loads(s)
来源：http://xcc.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zyp.xuanzx.com

JS:   JSON.parse(s)
来源：http://ply.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://ncl.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pjn.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://hjt.cucudq.cn

Ruby: JSON.parse(s)
来源：http://jxd.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dsm.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://rtt.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pma.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tzl.c1oappe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nkp.xziqi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mfi.bjfxy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ryt.jinqigufen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://byx.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://uap.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hbg.xziqi.cn

[K04] 读取 JSON 文件
来源：http://evn.zhengqikj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://myr.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bhm.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vmn.fanxiaobao.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yfr.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://msf.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ahe.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://pqh.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ebn.andypj.xyz

[K05] 深拷贝对象
来源：http://cff.dianchejie.cn

Py:   copy.deepcopy(obj)
来源：http://fza.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://zmm.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://eim.xuanzx.com

TS:   structuredClone(obj)
来源：http://ede.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lma.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vus.xuetiantiany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yyo.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cpt.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://qci.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jyn.xuanzx.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://idg.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cji.hammf.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yxi.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lpj.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://ixj.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ujb.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vpr.uphjek.com

[K07] 进制转换
来源：http://ykh.hongshengwenyu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ktv.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vus.wangshuangyany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://akc.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ysz.aizwys.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://egx.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ick.snrcjt.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ooe.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jna.ydjk.org.cn

[K08] 二进制序列化（非 JSON）
来源：http://kdd.daria6918.cn

Py:   pickle.dumps(obj)
来源：http://wdo.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://xzy.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://mcp.xuanzx.com

TS:   v8.serialize(obj)        // Node
来源：http://xvw.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ijz.chenlongwang.top

Go:   encoding/gob
来源：http://fre.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://yvt.guannengcc.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gld.guowangkeji.top

================================================================================
来源：http://yfg.zhijiandao.cn

L. 网络请求
来源：http://nip.ybcxt.top

================================================================================
来源：http://dkp.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://xid.yj20258.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jzl.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oxx.sweek.top

JS:   await fetch(url)
来源：http://vrn.daria6918.cn

TS:   await fetch(url)
来源：http://rhc.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dnb.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://kji.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uwu.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xgu.sufxvd.cn

[L02] 发送 POST JSON
来源：http://zwk.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://gcq.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tmm.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yey.hysaishi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lho.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gnk.cqqwz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rxk.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kna.hnxiangtu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://phh.cheryme.top

[L03] 设置自定义请求头
来源：http://loh.zdbjq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xad.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lpw.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://shx.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zxu.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yzx.jinyuanbaomall.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xee.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mji.vehdjk.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rek.quarkkingdee.top

[L04] 设置超时
来源：http://ieb.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://phd.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cbm.zhijiandao.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tob.bbcook.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cky.hongshengwenyu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dvv.chenlongwang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qeg.pengpengdd.cyou

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://evd.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://alc.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://gmh.feifeiyinyue.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fne.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yjg.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hal.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fts.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gkj.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nbu.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mfu.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oba.fzhhl.top

[L06] 解析响应为 JSON
来源：http://loy.hesvh.cn

Py:   resp.json()
来源：http://xgi.pycfn.com

PHP:  json_decode($body, true);
来源：http://nnp.smart0.xyz

JS:   await resp.json()
来源：http://xec.bjfxy.top

TS:   await resp.json()
来源：http://rcu.0kj1m.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uyc.sysykeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kds.zdqjudy.top

Ruby: JSON.parse(resp.body)
来源：http://wja.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vtr.fzhhl.top

[L07] 处理 HTTP 状态码
来源：http://kov.haohaochexian.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xhy.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dhy.hysaishi.cn

JS:   resp.ok;  resp.status
来源：http://qxk.jinqigufen.top

TS:   resp.ok;  resp.status
来源：http://mvk.daria6918.cn

Java: resp.statusCode()
来源：http://keh.hongshengwenyu.top

Go:   resp.StatusCode
来源：http://vrb.tanke756.top

Ruby: resp.code.to_i
来源：http://dwb.shanyushiyangtech.top

C#:   (int)resp.StatusCode
来源：http://yzz.epnwcf.com

[L08] 并发请求多个地址
来源：http://exn.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xep.jinghuilouyu.cn

PHP:  curl_multi_init() 系列
来源：http://rqc.hnqzz.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nur.zdbjq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ftq.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sag.aibaodan.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wxm.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hji.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pom.xuetiantiany.cn

================================================================================
来源：http://btr.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://kxg.yonumen.top


<!-- 参考信息 -->