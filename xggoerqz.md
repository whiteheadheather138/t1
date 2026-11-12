代发 wailian999

================================================================================
来源：http://bry.ppjwa.cn

I. 正则表达式
来源：http://gzv.tianlin.xyz

================================================================================
来源：http://zur.yfazqb.com

[I01] 判断是否匹配
来源：http://zbe.ctjpmb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qvh.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://kbr.tarul.cn

JS:   /\d+/.test(s)
来源：http://dky.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://slb.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cni.52xcode.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qhf.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://mdb.vqdsnc.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xfc.jyoumei.cn

[I02] 提取所有匹配
来源：http://brf.redwolf501.top

Py:   re.findall(r"\d+", s)
来源：http://qtm.yongpay.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xdb.yuxming.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wpl.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://lfr.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ccv.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ean.sjlbkw.cn

Ruby: s.scan(/\d+/)
来源：http://blc.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bdk.mhx1999.top

[I03] 提取捕获分组
来源：http://gdc.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gkd.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tsh.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gmh.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fyd.zhaomingkeji.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://itx.nwbrower.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://khl.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gyi.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pvm.svipenyu.cn

[I04] 正则替换
来源：http://evg.nwbrower.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nkh.haohaochexian.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ziz.ywan-chungtsiang.top

JS:   s.replace(/\d+/g, "#")
来源：http://jfg.zhoulong.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://aan.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://euw.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xyg.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://flq.hysaishi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xhb.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://oht.fengsongda.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lbb.daria6918.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kfu.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://jol.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://pxu.birdmap.top

Java: s.split("\\s*,\\s*")
来源：http://ccw.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ekv.chenzaomai.com

Ruby: s.split(/\s*,\s*/)
来源：http://yur.haohaochexian.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rkh.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ypq.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://koq.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wot.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jlf.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fyv.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://spb.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lma.gotoacloud.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kgr.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xqf.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://gqb.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mky.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xxq.cdnleiting.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wno.hnqzz.top

TS:   /error/gim
来源：http://mry.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yek.zycfv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://suu.ydjk.org.cn

Ruby: s.scan(/error/i)
来源：http://tjf.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cpi.jiagoushi.top

[I08] 贪婪与非贪婪匹配
来源：http://ice.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://elg.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gdb.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fqb.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xus.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rdn.yangfankeji.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rzl.hesvh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aow.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://svv.tarul.cn

================================================================================
来源：http://alg.cheryme.top

J. 日期与时间
来源：http://xnd.chenlongwang.top

================================================================================
来源：http://xfm.birdmap.top

[J01] 获取当前时间
来源：http://mbq.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fbq.fzhhl.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eqo.hammf.cn

JS:   new Date();  Date.now()
来源：http://dse.yuxming.cn

TS:   new Date();  Date.now()
来源：http://qze.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://dbl.52xcode.cn

Go:   time.Now()
来源：http://jvz.xuanzx.com

Ruby: Time.now
来源：http://rwd.hysaishi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qiq.yonumen.top

[J02] 格式化输出
来源：http://vwb.ivvv.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://awm.zhixingplan.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rwn.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ylf.tanke756.top

TS:   d.toISOString()
来源：http://ape.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://znx.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ylk.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://brp.ydzc1.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vsk.sysykeji.top

[J03] 字符串解析为日期
来源：http://rqc.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bvq.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ozc.tanke756.top

JS:   new Date("2024-01-02")
来源：http://ivi.ehwqpu.com

TS:   new Date("2024-01-02")
来源：http://vfk.jlsjyb.cn

Java: LocalDate.parse("2024-01-02")
来源：http://roo.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nok.fktsv.cn

Ruby: Date.parse("2024-01-02")
来源：http://gwh.hesvh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lat.haohaochexian.top

[J04] 时间戳与日期互转
来源：http://sul.chenzaomai.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jpw.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uea.smart0.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lsw.cashguo.top

TS:   Math.floor(Date.now() / 1000)
来源：http://iru.tanke756.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fnu.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cyx.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uih.jinyuanbaomall.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ntm.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://wnb.redwolf501.top

Py:   now + timedelta(days=7)
来源：http://skv.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ffc.yongpay.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lbh.smart0.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://piv.zhijiandao.cn

Java: LocalDate.now().plusDays(7)
来源：http://oup.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dmd.xziqi.cn

Ruby: Time.now + 7 * 86400
来源：http://vdo.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://koc.shanyushiyangtech.top

[J06] 计算两时间之差
来源：http://rdl.xinyue.icu

Py:   (end - start).total_seconds()
来源：http://fmu.bbcook.cn

PHP:  $end->diff($start)->days;
来源：http://gor.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yly.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eii.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lvz.ivvv.top

Go:   end.Sub(start).Hours()
来源：http://uyv.ctjpmb.com

Ruby: end - start                 # 返回秒数
来源：http://dwe.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://lbo.jiagoushi.top

[J07] 比较两个日期
来源：http://opm.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://epj.jiagoushi.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zch.chenzaomai.com

JS:   d1.getTime() < d2.getTime()
来源：http://moi.jinqigufen.top

TS:   d1.getTime() < d2.getTime()
来源：http://fwk.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uwf.birdmap.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vui.bjfxy.top

Ruby: d1 < d2;  d1 == d2
来源：http://bhr.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://rmy.zdqjudy.top

[J08] 提取年月日与星期
来源：http://cfz.dianchejie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ndh.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vbi.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sxb.nanxinkj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://min.dashuyun.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wgv.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://trk.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lhh.sjlbkw.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cin.yj202588.top

[J09] 时区处理
来源：http://cjd.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://npm.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uro.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jlh.shangyingyoupin.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cfl.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ago.zdqjudy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bep.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://urs.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://euc.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://htv.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ees.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hdu.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zec.gaohongyu789.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gro.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mjr.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tuz.ivvv.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tbb.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://seb.xuetiantiany.cn

================================================================================
来源：http://gpt.fehbvm.com

K. JSON 与序列化
来源：http://gwu.jyoumei.cn

================================================================================
来源：http://hlq.fktsv.cn

[K01] 对象转 JSON 字符串
来源：http://ump.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dpi.hywenlv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xqr.hammf.cn

JS:   JSON.stringify(obj)
来源：http://jlh.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://dio.kuanghao11.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mtb.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://ien.iojbl.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pyh.meibo888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cpb.zdbjq.cn

[K02] JSON 字符串转对象
来源：http://ldk.havefunace.top

Py:   json.loads(s)
来源：http://qkk.kuanghao11.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vxq.hesvh.cn

JS:   JSON.parse(s)
来源：http://uyy.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://bdn.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ndc.jyoumei.cn

Go:   json.Unmarshal(data, &v)
来源：http://ofl.gotoacloud.top

Ruby: JSON.parse(s)
来源：http://jat.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://way.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://fzl.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cxz.fengsongda.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wsp.yangfankeji.com

JS:   JSON.stringify(obj, null, 2)
来源：http://mch.vqdsnc.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hgf.cashguo.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gzm.hcnkem.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zat.tanke756.top

Ruby: JSON.pretty_generate(obj)
来源：http://ulh.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ble.hammf.cn

[K04] 读取 JSON 文件
来源：http://msj.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uyl.mhx1999.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eed.dashuyun.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://byy.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lag.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://acf.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://awl.zhoulong.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://wzp.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://adf.9152youxi.cn

[K05] 深拷贝对象
来源：http://amh.havefunace.top

Py:   copy.deepcopy(obj)
来源：http://xsv.nanxinkj.top

PHP:  unserialize(serialize($obj));
来源：http://nku.wangshuangyany.cn

JS:   structuredClone(obj)
来源：http://xzq.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://kxv.shuidangran.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nxx.52xcode.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nwf.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://czz.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wfc.daria6918.cn

[K06] 解析 URL 查询串
来源：http://nvx.sysykeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qdg.zdbjq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hsp.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hws.chenzaomai.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hil.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pnb.iojbl.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qxv.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yeo.gaohongyu789.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gui.zhoulong.xyz

[K07] 进制转换
来源：http://qgp.pengpengdd.cyou

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vqw.meibo888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qij.xuanzx.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nbp.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ghr.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://psg.cucudq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lcl.yj202588.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uwh.vqdsnc.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ipv.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://jfa.havefunace.top

Py:   pickle.dumps(obj)
来源：http://wee.tarul.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ooa.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://dlt.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://hya.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ivb.yj20258888.top

Go:   encoding/gob
来源：http://lfn.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://tww.52xcode.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xtu.andypj.xyz

================================================================================
来源：http://noo.gzhubu.top

L. 网络请求
来源：http://pfc.epnwcf.com

================================================================================
来源：http://bjn.jqgfzy.top

[L01] 发送 GET 请求
来源：http://hxy.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ztm.chenzaomai.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uvi.cheryme.top

JS:   await fetch(url)
来源：http://mou.mhx1999.top

TS:   await fetch(url)
来源：http://hqv.vehdjk.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rlo.fengsongda.top

Go:   resp, err := http.Get(url)
来源：http://gxr.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jur.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xpi.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://pii.daxiang520.top

Py:   requests.post(url, json={"a": 1})
来源：http://ueg.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pgo.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tpb.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://upp.pycfn.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wxa.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://viy.meibo888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://weh.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iyy.svipenyu.cn

[L03] 设置自定义请求头
来源：http://ewl.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kco.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uql.zdbjq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bco.shuidangran.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://evf.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nhd.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tpy.daxiang520.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dmm.vehdjk.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vtg.ywan-chungtsiang.top

[L04] 设置超时
来源：http://uan.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://oqf.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ifz.hnqzz.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lul.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bkx.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://twy.ybcxt.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mao.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fhi.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qds.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://hum.chenjidiqi.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xhx.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cpw.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://trf.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://idk.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tjy.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eio.ctjpmb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://civ.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rgi.jinghuilouyu.cn

[L06] 解析响应为 JSON
来源：http://rqx.vqdsnc.cn

Py:   resp.json()
来源：http://kcp.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://jrx.ydjk.org.cn

JS:   await resp.json()
来源：http://unl.shanyushiyangkeji.top

TS:   await resp.json()
来源：http://tnw.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qli.jinqigfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nun.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://lax.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ssh.zycfv.cn


<!-- 参考信息 -->