代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xsc.52xcode.cn

[I03] 提取捕获分组
来源：http://mdl.hnxiangtu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ybe.pycfn.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ypm.gogol.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ozh.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dkd.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ovf.gaohongyu789.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pfr.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wht.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cza.quarkkingdee.top

[I04] 正则替换
来源：http://hex.xingfuxueyuan.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://snh.iojbl.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zdc.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wgf.hesvh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wbl.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://wqr.jinqigufen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://moi.vehdjk.com

Ruby: s.gsub(/\d+/, "#")
来源：http://hoy.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zyk.ppjwa.cn

[I05] 按正则拆分
来源：http://doe.hammf.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://eul.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ybx.chenjidiqi.icu

JS:   s.split(/\s*,\s*/)
来源：http://zrl.vqdsnc.cn

TS:   s.split(/\s*,\s*/)
来源：http://bum.cdnleiting.top

Java: s.split("\\s*,\\s*")
来源：http://pam.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hsr.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://clg.smart0.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zev.bjfxy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ame.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yxu.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fyh.iojbl.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aej.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ygs.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xbr.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mab.hysaishi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bkh.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nsb.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://mht.wangshuangyany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ljj.svipenyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kgn.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://udx.yonumen.top

TS:   /error/gim
来源：http://cpz.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vnr.xziqi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fyf.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://pnc.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vrh.haohaochexian.top

[I08] 贪婪与非贪婪匹配
来源：http://rhn.chenjidiqi.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ygl.aibaodan.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gpk.52xcode.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mxg.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bix.sysykeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://krl.ctjpmb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://snu.gotoacloud.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://afc.aizwys.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wmz.wangdashe.top

================================================================================
来源：http://frm.guannengcc.top

J. 日期与时间
来源：http://hzm.dianchejie.cn

================================================================================
来源：http://ayh.zhoulong.xyz

[J01] 获取当前时间
来源：http://mhs.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pon.tanke756.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wzh.feifeiyinyue.top

JS:   new Date();  Date.now()
来源：http://rbn.bbcook.cn

TS:   new Date();  Date.now()
来源：http://goz.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://eeg.hesvh.cn

Go:   time.Now()
来源：http://sfb.nanxuanxn.top

Ruby: Time.now
来源：http://hbz.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cri.hnqzz.top

[J02] 格式化输出
来源：http://jni.gogol.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hty.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://efn.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://szn.yvedp.cn

TS:   d.toISOString()
来源：http://xfm.jinyuanbaomall.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://juq.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tqs.hnqzz.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://siy.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jjm.birdmap.top

[J03] 字符串解析为日期
来源：http://mfp.zhiwuduotai.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ewz.gogol.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qvc.aibaodan.cn

JS:   new Date("2024-01-02")
来源：http://yfp.snrcjt.cn

TS:   new Date("2024-01-02")
来源：http://bcs.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kaz.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pug.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://swh.shzxlz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bxx.yongpay.top

[J04] 时间戳与日期互转
来源：http://foe.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://igd.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hng.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nag.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pwj.vehdjk.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xmm.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iqz.nanxinkj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vwv.zhiwuduotai.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bap.ctjpmb.com

[J05] 时间加减（加 7 天）
来源：http://osp.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://cnf.jqgfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gxc.cucudq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://isd.xylfe.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xtq.jqgfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://bur.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://raw.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://lxz.cashguo.top

C#:   DateTime.Now.AddDays(7)
来源：http://vfa.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://wyp.cheryme.top

Py:   (end - start).total_seconds()
来源：http://rsw.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://kum.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ily.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uuo.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ayi.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://zik.dianchejie.cn

Ruby: end - start                 # 返回秒数
来源：http://lwn.tarul.cn

C#:   (end - start).TotalSeconds
来源：http://pty.haohaochexian.top

[J07] 比较两个日期
来源：http://whg.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://pvw.jinghuilouyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ghi.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://ppc.xuetiantiany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fef.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xfu.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lca.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://rsf.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://aqu.jqgfzy.top

[J08] 提取年月日与星期
来源：http://zte.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cyg.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://okz.epnwcf.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fhj.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vqf.redwolf501.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hhe.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gst.dashuyun.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gcz.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hqt.zhijiandao.cn

[J09] 时区处理
来源：http://xgp.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kha.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://phb.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yag.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vno.quarkkingdee.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xjz.quarkkingdee.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lmk.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hmy.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hrx.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://xcl.hcnkem.com

Py:   date.today();  date.today().replace(day=1)
来源：http://nnm.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bxj.gaohongyu789.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qbq.hnxiangtu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hup.hysaishi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pfa.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://joe.aizwys.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xig.ydjk.org.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nov.yangfankeji.com

================================================================================
来源：http://qvy.xingfuxueyuan.xyz

K. JSON 与序列化
来源：http://xyg.jiagoushi.top

================================================================================
来源：http://fos.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://wnv.c1oappe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mkv.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fgv.xziqi.cn

JS:   JSON.stringify(obj)
来源：http://blu.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://wuz.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hui.cashguo.top

Go:   json.Marshal(obj)
来源：http://hfk.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yor.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kde.tianlin.xyz

[K02] JSON 字符串转对象
来源：http://nsd.wangshuangyany.cn

Py:   json.loads(s)
来源：http://ifk.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vnt.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://vtj.shzxlz.cn

TS:   JSON.parse(s)
来源：http://gou.gaohongyu789.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vcg.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://jrm.vehdjk.com

Ruby: JSON.parse(s)
来源：http://yua.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ehu.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://pnw.guannengcc.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cmk.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xvo.ppjwa.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zzx.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vhh.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zfo.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zlv.tian-w.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ebf.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ymu.dianchejie.cn

[K04] 读取 JSON 文件
来源：http://bvp.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qgj.yonumen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tct.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wxl.sjlbkw.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gmw.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hrp.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qqq.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zpa.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sle.nwbrower.top

[K05] 深拷贝对象
来源：http://ydx.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://iky.yangfankeji.com

PHP:  unserialize(serialize($obj));
来源：http://bfi.ivvv.top

JS:   structuredClone(obj)
来源：http://gib.zdqjudy.top

TS:   structuredClone(obj)
来源：http://hpb.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ums.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ifi.daria6918.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jkb.jinghuilouyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dbz.meibo888.top

[K06] 解析 URL 查询串
来源：http://dlo.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://utz.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hhk.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://inb.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fhp.zdbjq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nes.aizwys.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tzc.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://imu.fehbvm.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rjt.9152youxi.cn

[K07] 进制转换
来源：http://rrx.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sdr.zycfv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qqb.svipenyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nbz.dashuyun.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dzo.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rio.tanke756.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xvu.kuanghao11.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ihb.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://weo.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://cmc.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://nqa.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cpa.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://bbs.jqgufenzy.top

TS:   v8.serialize(obj)        // Node
来源：http://uto.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://klu.shangyingyoupin.top

Go:   encoding/gob
来源：http://xfa.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://ppx.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kyy.zycfv.cn

================================================================================
来源：http://zkp.zhaomingkeji.xyz

L. 网络请求
来源：http://azi.316326.xyz

================================================================================
来源：http://skc.sxryk.cn

[L01] 发送 GET 请求
来源：http://ruk.yongpay.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xhu.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yrf.nanxuanxn.top

JS:   await fetch(url)
来源：http://lsb.svipenyu.cn

TS:   await fetch(url)
来源：http://oso.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://frs.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://hht.hywenlv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qkx.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ahq.yuxming.cn

[L02] 发送 POST JSON
来源：http://ibl.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://qur.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mnd.hysaishi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rwc.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://puz.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hst.quarkkingdee.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tcl.shanyushiyangtech.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ead.yueranfly.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mwa.nwbrower.top

[L03] 设置自定义请求头
来源：http://pbm.fzhhl.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mvz.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ahs.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tic.aizwys.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uwu.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zoc.daxiang520.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dje.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wvj.xinyue.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mdf.yuanzhike.top

[L04] 设置超时
来源：http://gev.yj20258.top

Py:   requests.get(url, timeout=5)
来源：http://lma.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wtc.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lpm.fanxiaobao.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wsp.andypj.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eks.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uin.chenlongwang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lvn.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fog.nanxinkj.top

[L05] 上传文件（multipart）
来源：http://rla.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ref.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zaq.jinghuilouyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bbt.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ykg.yj202588.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fro.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pic.xuanzx.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tuy.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qxx.9152youxi.cn

[L06] 解析响应为 JSON
来源：http://mvk.fanxiaobao.xyz

Py:   resp.json()
来源：http://ybt.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://wdv.shuidangran.top

JS:   await resp.json()
来源：http://rcp.iojbl.cn

TS:   await resp.json()
来源：http://hck.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qow.smart0.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hxo.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://yvp.cqqwz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ckl.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://fof.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ccw.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://neq.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://rba.havefunace.top

TS:   resp.ok;  resp.status
来源：http://ygc.fktsv.cn

Java: resp.statusCode()
来源：http://njq.ctjpmb.com

Go:   resp.StatusCode
来源：http://spe.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://utw.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://qqc.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://spz.tarul.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jrv.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://vkv.xuanzx.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vtf.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ucr.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ukv.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kom.snrcjt.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zfr.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tio.jinghuilouyu.cn

================================================================================
来源：http://pjq.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://vcv.cheryme.top


<!-- 参考信息 -->