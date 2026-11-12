代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rze.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://kfl.hcnkem.com

JS:   /\d+/.test(s)
来源：http://win.epnwcf.com

TS:   /\d+/.test(s)
来源：http://tkx.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ist.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ysk.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://rgs.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gvn.shuidangran.top

[I02] 提取所有匹配
来源：http://nzy.hywenlv.cn

Py:   re.findall(r"\d+", s)
来源：http://ecb.shanyushiyangtech.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gfy.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uxh.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://nlk.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vqf.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tlw.wangdashe.top

Ruby: s.scan(/\d+/)
来源：http://lmd.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mxb.zhoulong.xyz

[I03] 提取捕获分组
来源：http://ptq.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dey.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jug.andypj.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vfo.ctjpmb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://axf.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wet.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bom.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dah.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uos.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://thb.yuanzhike.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jpg.xziqi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sni.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://olr.tanke756.top

TS:   s.replace(/\d+/g, "#")
来源：http://olz.fanxiaobao.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://yde.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hxy.hnqzz.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cty.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ypd.smart0.xyz

[I05] 按正则拆分
来源：http://wgi.xuanzx.com

Py:   re.split(r"\s*,\s*", s)
来源：http://aec.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://apf.tian-w.cn

JS:   s.split(/\s*,\s*/)
来源：http://fvn.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://vum.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://dtk.quarkkingdee.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nxm.tian-w.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fdd.ydjk.org.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fah.jiagoushi.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pxm.mhx1999.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nwh.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dka.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xlh.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nbi.yueranfly.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xcu.zycfv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yth.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://igp.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://szi.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://whr.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zbd.0kj1m.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://odp.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yva.birdmap.top

TS:   /error/gim
来源：http://abv.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cuk.iojbl.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sce.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://qmx.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cjk.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://zwo.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://klj.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xez.nwbrower.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://foh.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iqh.hnxiangtu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vmt.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hot.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://imc.hnqzz.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vjs.ydjk.org.cn

================================================================================
来源：http://uvs.jinqigfzy.top

J. 日期与时间
来源：http://gry.wangdashe.top

================================================================================
来源：http://xyi.hammf.cn

[J01] 获取当前时间
来源：http://iip.iojbl.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://inm.sweek.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fgd.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://yis.c1oappe.top

TS:   new Date();  Date.now()
来源：http://afo.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ocb.xingfuxueyuan.xyz

Go:   time.Now()
来源：http://idy.shanyushiyangtech.top

Ruby: Time.now
来源：http://zju.wangshuangyany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ftx.jinqigufen.top

[J02] 格式化输出
来源：http://iyn.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ifu.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mbq.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ytj.svipenyu.cn

TS:   d.toISOString()
来源：http://xus.daxiang520.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nra.chenlongwang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bdd.xylfe.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hna.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ydd.wangshuangyany.cn

[J03] 字符串解析为日期
来源：http://ttv.epnwcf.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://crj.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mtg.316326.xyz

JS:   new Date("2024-01-02")
来源：http://yqr.chenzaomai.com

TS:   new Date("2024-01-02")
来源：http://jzd.hnqzz.top

Java: LocalDate.parse("2024-01-02")
来源：http://hyt.jlsjyb.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bha.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://avv.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sgf.wangdashe.top

[J04] 时间戳与日期互转
来源：http://lbt.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://far.xinyue.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sju.ywan-chungtsiang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kyd.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hjs.ydjk.org.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kcc.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gis.andypj.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dlk.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ovj.hywenlv.cn

[J05] 时间加减（加 7 天）
来源：http://lzb.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://tya.ydjk.org.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cpu.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ceg.gzhubu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aua.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://alr.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pbf.52xcode.cn

Ruby: Time.now + 7 * 86400
来源：http://jvg.jyoumei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ruh.xziqi.cn

[J06] 计算两时间之差
来源：http://ptx.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://hme.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://yxr.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://npu.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://stw.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yra.iojbl.cn

Go:   end.Sub(start).Hours()
来源：http://jcb.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://ezh.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://kue.yuxming.cn

[J07] 比较两个日期
来源：http://oqq.sufxvd.cn

Py:   d1 < d2;  d1 == d2
来源：http://dqq.cheryme.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jyq.uphjek.com

JS:   d1.getTime() < d2.getTime()
来源：http://rhs.jqgufenzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://qon.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xbz.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rhc.tanke756.top

Ruby: d1 < d2;  d1 == d2
来源：http://nnr.birdmap.top

C#:   d1 < d2;  d1 == d2
来源：http://iln.jinqigufen.top

[J08] 提取年月日与星期
来源：http://rcu.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mxa.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uim.redwolf501.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://neo.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://erk.mhx1999.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://erd.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vua.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tza.jqgfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hkz.zhengqikj.top

[J09] 时区处理
来源：http://rmm.ydzc1.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mbr.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lkm.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xje.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jof.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oug.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xru.chenjidiqi.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://lpi.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tik.nanxuanxn.top

[J10] 取今天 / 本月第一天
来源：http://dbh.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wdm.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mpw.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qxt.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vdt.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ngb.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dei.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mva.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qny.nanxuanxn.top

================================================================================
来源：http://bso.chenlongwang.top

K. JSON 与序列化
来源：http://wqm.hfpthk.cn

================================================================================
来源：http://cav.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://faz.ywan-chungtsiang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ogs.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://moa.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://zsk.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://end.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qcf.fehbvm.com

Go:   json.Marshal(obj)
来源：http://rtc.xuetiantiany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kue.tianlin.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://yup.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://gtu.hnqzz.top

Py:   json.loads(s)
来源：http://jlx.chenlongwang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://msj.ctjpmb.com

JS:   JSON.parse(s)
来源：http://och.guannengcc.top

TS:   JSON.parse(s)
来源：http://sry.vqdsnc.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fma.sjlbkw.cn

Go:   json.Unmarshal(data, &v)
来源：http://ksv.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://kem.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gly.xingfuxueyuan.xyz

[K03] JSON 美化输出（带缩进）
来源：http://ein.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xtm.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uyc.sjlbkw.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zzm.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wbj.shuidangran.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wzz.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://crc.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://cjx.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sgj.chenlongwang.top

[K04] 读取 JSON 文件
来源：http://xxj.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dol.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kmn.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uts.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cpb.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wae.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qdl.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lbz.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nmy.xylfe.cn

[K05] 深拷贝对象
来源：http://czd.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://dvo.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://hsg.pengpengdd.cyou

JS:   structuredClone(obj)
来源：http://vhm.ivvv.top

TS:   structuredClone(obj)
来源：http://ggc.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iqs.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vln.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zqv.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mum.svipenyu.cn

[K06] 解析 URL 查询串
来源：http://svv.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://odo.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rgu.xuetiantiany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xto.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hkn.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nbm.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cgk.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bjk.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ohu.guannengcc.top

[K07] 进制转换
来源：http://seb.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dqc.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://quj.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wrx.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://esv.fengsongda.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://myr.andypj.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wdh.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jho.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://txs.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://ibk.jlsjyb.cn

Py:   pickle.dumps(obj)
来源：http://qlq.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dkx.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://tqq.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://fwn.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://img.yongpay.top

Go:   encoding/gob
来源：http://dio.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://pnm.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wgj.hywenlv.cn

================================================================================
来源：http://pue.andypj.xyz

L. 网络请求
来源：http://fzo.sysykeji.top

================================================================================
来源：http://ocj.jinqigufen.top

[L01] 发送 GET 请求
来源：http://yeo.gogol.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vzo.yongpay.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cnb.kuanghao11.cn

JS:   await fetch(url)
来源：http://bvc.guowangkeji.top

TS:   await fetch(url)
来源：http://bdd.tarul.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xrr.chenzaomai.com

Go:   resp, err := http.Get(url)
来源：http://zgw.ybcxt.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qfp.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ade.bjfxy.top

[L02] 发送 POST JSON
来源：http://yxx.cucudq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://euj.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ogb.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iat.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rci.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jvp.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pgy.jinghuilouyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rfw.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gfz.ydzc1.top

[L03] 设置自定义请求头
来源：http://afk.shuidangran.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lnx.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vid.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yiz.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://slp.316326.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ngx.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fik.hongshengwenyu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nmh.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cix.jinqigufen.top

[L04] 设置超时
来源：http://jej.yfazqb.com

Py:   requests.get(url, timeout=5)
来源：http://sms.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://roz.chenlongwang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tgd.pengpengdd.cyou

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wfh.bjfxy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lhr.xingfuxueyuan.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cbd.dashuyun.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jvc.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bws.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://oot.zycfv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wbq.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ugg.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ywm.xuanzx.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ksg.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bws.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ihg.epnwcf.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iat.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pla.gzhubu.top

[L06] 解析响应为 JSON
来源：http://hzh.haohaochexian.top

Py:   resp.json()
来源：http://okz.ydzc1.top

PHP:  json_decode($body, true);
来源：http://glf.yvedp.cn

JS:   await resp.json()
来源：http://wyq.hywenlv.cn

TS:   await resp.json()
来源：http://dys.shuidangran.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qis.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mim.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://qlz.gaohongyu789.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mjh.c1oappe.top

[L07] 处理 HTTP 状态码
来源：http://bzm.jiagoushi.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eku.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xqo.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://kea.zhongyouzk.top


<!-- 参考信息 -->