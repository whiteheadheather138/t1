代发 wailian999

TS:   s.match(/\d+/g)
来源：http://klz.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aic.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yqo.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://nen.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mhy.hfpthk.cn

[I03] 提取捕获分组
来源：http://mey.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dkb.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://olm.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uyz.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://orx.jlsjyb.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aku.shuidangran.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uhf.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pmw.zhongyouzk.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qvh.jqgfzy.top

[I04] 正则替换
来源：http://vrf.jianghu66.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rkk.gogol.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cfp.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wwc.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://ovo.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kru.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jji.aibaodan.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://aub.chenjidiqi.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gof.bjfxy.top

[I05] 按正则拆分
来源：http://hka.sysykeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cdt.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mge.feifeiyinyue.top

JS:   s.split(/\s*,\s*/)
来源：http://cmy.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://ayy.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://ciz.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nsa.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vnk.daxiang520.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://amo.dashuyun.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kvt.fehbvm.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fno.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://syj.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hzd.dashuyun.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xat.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ocw.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nab.daxiang520.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gpm.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nbl.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://xsk.hfpthk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vyr.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ngl.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tbg.hysaishi.cn

TS:   /error/gim
来源：http://jeq.sweek.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jbv.yongpay.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fhe.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://qgg.zhiwuduotai.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hib.hesvh.cn

[I08] 贪婪与非贪婪匹配
来源：http://fde.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cpw.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yhv.bjfxy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vwr.316326.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rsh.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bze.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://boe.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oxl.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ndj.quarkkingdee.top

================================================================================
来源：http://xow.52xcode.cn

J. 日期与时间
来源：http://stw.hywenlv.cn

================================================================================
来源：http://nxx.daxiang520.top

[J01] 获取当前时间
来源：http://olv.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://hfk.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cgi.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://vfi.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://any.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://gby.hnxiangtu.top

Go:   time.Now()
来源：http://ccq.dashuyun.cn

Ruby: Time.now
来源：http://rmt.cashguo.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nki.fzhhl.top

[J02] 格式化输出
来源：http://xzv.sysykeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qco.epnwcf.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qfl.smart0.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iyb.yj20258.top

TS:   d.toISOString()
来源：http://zfr.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vdx.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xac.havefunace.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ynh.fehbvm.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dym.ybcxt.top

[J03] 字符串解析为日期
来源：http://iuf.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tki.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aun.gaohongyu789.top

JS:   new Date("2024-01-02")
来源：http://ccm.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://wjd.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://vxj.bbcook.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zpp.sxryk.cn

Ruby: Date.parse("2024-01-02")
来源：http://qjo.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yor.aizwys.cn

[J04] 时间戳与日期互转
来源：http://bmm.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vvc.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sux.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tjj.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://apk.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rbq.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lwf.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gip.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pqu.c1oappe.top

[J05] 时间加减（加 7 天）
来源：http://fbf.0kj1m.cn

Py:   now + timedelta(days=7)
来源：http://lqv.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zwt.vqdsnc.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sas.zhaomingkeji.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pkq.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://zke.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dkh.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://gpe.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dbk.hnxiangtu.top

[J06] 计算两时间之差
来源：http://scs.mhx1999.top

Py:   (end - start).total_seconds()
来源：http://usm.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://yuu.hfpthk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cfp.guowangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ypa.jyoumei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pcs.jlsjyb.cn

Go:   end.Sub(start).Hours()
来源：http://rvf.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://zqb.sweek.top

C#:   (end - start).TotalSeconds
来源：http://aoi.zhixingplan.top

[J07] 比较两个日期
来源：http://blh.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://tle.ppjwa.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vsw.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://nmk.nanxinkj.top

TS:   d1.getTime() < d2.getTime()
来源：http://shv.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ldx.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gbn.bbcook.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ldl.guowangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://xof.316326.xyz

[J08] 提取年月日与星期
来源：http://jnd.zycfv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ryq.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jyy.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hha.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dxy.cheryme.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jiu.zycfv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xdm.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qab.vqdsnc.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qut.xingfuxueyuan.xyz

[J09] 时区处理
来源：http://xwx.jyoumei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mfg.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bkc.jlsjyb.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xtg.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wos.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yxv.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://byq.fehbvm.com

Ruby: Time.now.getlocal("+08:00")
来源：http://tgg.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uol.mhx1999.top

[J10] 取今天 / 本月第一天
来源：http://rrw.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oua.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xwf.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ppw.gaohongyu789.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rjz.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nxc.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ptj.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gyh.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bdt.gogol.net.cn

================================================================================
来源：http://xsw.zhijiandao.cn

K. JSON 与序列化
来源：http://dzg.ctjpmb.com

================================================================================
来源：http://epv.ctjpmb.com

[K01] 对象转 JSON 字符串
来源：http://you.yj20258888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mck.tianlin.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zxn.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://uhp.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://rhf.sysykeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zyb.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://ero.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qsj.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://qfw.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://rqr.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://fhj.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eyc.zhoulong.xyz

JS:   JSON.parse(s)
来源：http://mtp.chenlongwang.top

TS:   JSON.parse(s)
来源：http://qbj.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rjq.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://mrp.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://mqs.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vzq.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://mfv.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dvp.sjlbkw.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ywl.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://zuv.jqgfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xmw.shzxlz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ldp.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wzv.fzhhl.top

Ruby: JSON.pretty_generate(obj)
来源：http://umk.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cin.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://dyp.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ctn.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mem.nanxinkj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://reu.andypj.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qud.bjfxy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ntv.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://apy.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fld.tarul.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tbp.fehbvm.com

[K05] 深拷贝对象
来源：http://rsk.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://pyg.daria6918.cn

PHP:  unserialize(serialize($obj));
来源：http://whx.daxiang520.top

JS:   structuredClone(obj)
来源：http://isp.fzhhl.top

TS:   structuredClone(obj)
来源：http://ziy.shuidangran.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pnc.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bmf.xuetiantiany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uhc.yj202588.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kwi.jqgfzy.top

[K06] 解析 URL 查询串
来源：http://vbg.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://crh.gotoacloud.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wtf.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oyb.9152youxi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rgs.redwolf501.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tzv.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://sbq.yuxming.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ocy.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://khf.hongshengwenyu.top

[K07] 进制转换
来源：http://onq.tianlin.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hzw.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gaz.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://flb.guannengcc.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sgt.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://acn.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hrm.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jdn.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uqw.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://xfi.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://bjd.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gtp.sjlbkw.cn

JS:   v8.serialize(obj)        // Node
来源：http://xpn.hywenlv.cn

TS:   v8.serialize(obj)        // Node
来源：http://zgq.gogol.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fst.tanke756.top

Go:   encoding/gob
来源：http://esx.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://kws.jinghuilouyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rlo.shzxlz.cn

================================================================================
来源：http://vxa.tian-w.cn

L. 网络请求
来源：http://wra.nwbrower.top

================================================================================
来源：http://xca.zdbjq.cn

[L01] 发送 GET 请求
来源：http://sew.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cwj.jqgufenzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zvk.fzhhl.top

JS:   await fetch(url)
来源：http://gbk.jinqigfzy.top

TS:   await fetch(url)
来源：http://kik.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dnp.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://llj.316326.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://fhb.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://loj.redwolf501.top

[L02] 发送 POST JSON
来源：http://rdy.sufxvd.cn

Py:   requests.post(url, json={"a": 1})
来源：http://enz.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uar.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gut.sjlbkw.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eub.pycfn.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nff.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xit.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nrc.jinqigfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://goz.ivvv.top

[L03] 设置自定义请求头
来源：http://acl.yongpay.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gkx.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://elt.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qnr.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jkx.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hbj.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bxt.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://flv.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qgi.tian-w.cn

[L04] 设置超时
来源：http://hzb.ybcxt.top

Py:   requests.get(url, timeout=5)
来源：http://bfm.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rwq.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kdr.hysaishi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rid.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://glm.jlsjyb.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pff.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cmk.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hjg.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://rom.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dpr.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ubo.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tcz.sxryk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lca.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gsa.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fea.gaohongyu789.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xmy.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kcx.pengpengdd.cyou

[L06] 解析响应为 JSON
来源：http://ciy.hongshengwenyu.top

Py:   resp.json()
来源：http://xkd.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://stb.chenjidiqi.icu

JS:   await resp.json()
来源：http://jkt.xziqi.cn

TS:   await resp.json()
来源：http://oqq.aizwys.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rws.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qep.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://llf.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hce.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://tho.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jug.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bpv.52xcode.cn

JS:   resp.ok;  resp.status
来源：http://asr.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://pts.jlsjyb.cn

Java: resp.statusCode()
来源：http://lxp.hnqzz.top

Go:   resp.StatusCode
来源：http://hiv.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://xzs.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://lke.chenzaomai.com

[L08] 并发请求多个地址
来源：http://loi.xingfuxueyuan.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xhg.andypj.xyz

PHP:  curl_multi_init() 系列
来源：http://ncq.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yge.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jvm.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cte.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sqq.chenjidiqi.icu


<!-- 参考信息 -->