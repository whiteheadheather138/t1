代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://uoz.aizwys.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nle.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://les.uphjek.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bjk.shanyushiyangtech.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://okj.quarkkingdee.top

Go:   defer f.Close()
来源：http://otr.fanxiaobao.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://deg.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bko.mhx1999.top

================================================================================
来源：http://wrf.guannengcc.top

I. 正则表达式
来源：http://bdw.yonumen.top

================================================================================
来源：http://moc.gzhubu.top

[I01] 判断是否匹配
来源：http://bdz.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cwp.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://qvz.xingfuxueyuan.xyz

JS:   /\d+/.test(s)
来源：http://bll.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://cgc.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://skx.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ezw.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://qhy.ydjk.org.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nzv.chenlongwang.top

[I02] 提取所有匹配
来源：http://bza.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://efj.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ktb.jianghu66.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vak.fzhhl.top

TS:   s.match(/\d+/g)
来源：http://dwo.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sfp.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ejt.jqgufenzy.top

Ruby: s.scan(/\d+/)
来源：http://lpe.smart0.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ikz.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://mjb.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wvj.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fxu.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yrj.zhixingplan.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://slb.sxryk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ytn.zycfv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iig.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kjl.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rvz.smart0.xyz

[I04] 正则替换
来源：http://ndm.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://afk.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cqj.hnqzz.top

JS:   s.replace(/\d+/g, "#")
来源：http://bjb.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://nex.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ezf.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fmu.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fsk.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uum.sysykeji.top

[I05] 按正则拆分
来源：http://gpg.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gdx.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ika.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://ipk.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://wkv.cheryme.top

Java: s.split("\\s*,\\s*")
来源：http://ebv.hcnkem.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fpu.hywenlv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hqo.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://utt.andypj.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vbg.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yly.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yqi.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://srq.jinyuanbaomall.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wrk.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xwq.sjlbkw.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iux.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://htc.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ael.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://jni.nwbrower.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xux.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xze.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uqi.52xcode.cn

TS:   /error/gim
来源：http://xag.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dnf.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jed.jiagoushi.top

Ruby: s.scan(/error/i)
来源：http://pze.jlsjyb.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kgx.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://qvf.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hmm.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://soh.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ifj.tian-w.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ghm.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nlp.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gmu.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://evi.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mrk.snrcjt.cn

================================================================================
来源：http://lwp.zhongyouzk.top

J. 日期与时间
来源：http://vug.yongpay.top

================================================================================
来源：http://tmx.sweek.top

[J01] 获取当前时间
来源：http://vah.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ped.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://grn.ybcxt.top

JS:   new Date();  Date.now()
来源：http://dtp.chenjidiqi.icu

TS:   new Date();  Date.now()
来源：http://mpm.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kby.birdmap.top

Go:   time.Now()
来源：http://qch.daria6918.cn

Ruby: Time.now
来源：http://oss.redwolf501.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xjf.mhx1999.top

[J02] 格式化输出
来源：http://tft.shanyushiyangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cqp.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qvu.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bkk.gogol.net.cn

TS:   d.toISOString()
来源：http://uxa.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xhv.xylfe.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kww.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://izj.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aaz.nanxuanxn.top

[J03] 字符串解析为日期
来源：http://ust.svipenyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hsx.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://llk.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://ncj.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://gcc.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://hbj.pengpengdd.cyou

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aiz.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://ogh.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://psx.aizwys.cn

[J04] 时间戳与日期互转
来源：http://cze.yfazqb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vlg.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eol.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hfv.xylfe.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yyz.zhaomingkeji.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iwm.vqdsnc.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dlt.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aff.zhiwuduotai.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lhf.cucudq.cn

[J05] 时间加减（加 7 天）
来源：http://dno.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://azi.shzxlz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iot.xuetiantiany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gfg.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vol.yj20258.top

Java: LocalDate.now().plusDays(7)
来源：http://uhn.nwbrower.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jub.316326.xyz

Ruby: Time.now + 7 * 86400
来源：http://aqt.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://ajg.zdqjudy.top

[J06] 计算两时间之差
来源：http://bqe.dashuyun.cn

Py:   (end - start).total_seconds()
来源：http://qta.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://nhi.dashuyun.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://trz.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vit.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://lhp.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://qdc.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://hpe.wangshuangyany.cn

C#:   (end - start).TotalSeconds
来源：http://jzs.jiagoushi.top

[J07] 比较两个日期
来源：http://kde.jinqigfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://bgz.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mjf.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hwh.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://tfn.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wji.cqqwz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wrn.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://xqd.gotoacloud.top

C#:   d1 < d2;  d1 == d2
来源：http://vxs.yonumen.top

[J08] 提取年月日与星期
来源：http://dye.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yxe.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xsi.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ads.9152youxi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mlx.aizwys.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mzu.yuanzhike.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uie.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mog.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hsf.wangshuangyany.cn

[J09] 时区处理
来源：http://ppz.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bct.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://und.zdbjq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rdm.gogol.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://udh.gaohongyu789.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jlu.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sty.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://blv.sjlbkw.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hds.ctjpmb.com

[J10] 取今天 / 本月第一天
来源：http://jrs.yonumen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lwf.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kol.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uup.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ewz.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tpe.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xms.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zjo.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qdc.aibaodan.cn

================================================================================
来源：http://amy.zhijiandao.cn

K. JSON 与序列化
来源：http://gla.bbcook.cn

================================================================================
来源：http://ldv.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://nxh.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zix.jinqigufen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ctr.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://nrf.smart0.xyz

TS:   JSON.stringify(obj)
来源：http://htc.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ywa.vehdjk.com

Go:   json.Marshal(obj)
来源：http://agc.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://eqx.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://jkh.zycfv.cn

[K02] JSON 字符串转对象
来源：http://dch.xylfe.cn

Py:   json.loads(s)
来源：http://mfx.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nsv.yuxming.cn

JS:   JSON.parse(s)
来源：http://meb.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://ogb.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://whh.vqdsnc.cn

Go:   json.Unmarshal(data, &v)
来源：http://pyu.xziqi.cn

Ruby: JSON.parse(s)
来源：http://kex.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lcx.yj202588.top

[K03] JSON 美化输出（带缩进）
来源：http://jny.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blm.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pxi.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bmz.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lhe.mhx1999.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nfs.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ofc.sufxvd.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hbq.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://umq.vqdsnc.cn

[K04] 读取 JSON 文件
来源：http://wbv.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iml.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zma.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aau.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qqo.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dwd.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wlv.zhongyouzk.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ncj.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uey.hfpthk.cn

[K05] 深拷贝对象
来源：http://ikm.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://rkg.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://vgj.52xcode.cn

JS:   structuredClone(obj)
来源：http://dok.epnwcf.com

TS:   structuredClone(obj)
来源：http://evu.fengsongda.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ncl.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iih.daria6918.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hew.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ved.cashguo.top

[K06] 解析 URL 查询串
来源：http://xxs.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uts.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gnv.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tcd.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fxo.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nrv.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://iya.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gvx.hesvh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ftk.vqdsnc.cn

[K07] 进制转换
来源：http://zep.sjlbkw.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oxs.yvedp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kap.fanxiaobao.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yed.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qay.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iht.316326.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yjw.ywan-chungtsiang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xvq.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tgc.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://vuy.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://kor.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ign.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://jrp.zdbjq.cn

TS:   v8.serialize(obj)        // Node
来源：http://dtz.xingfuxueyuan.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ikf.iojbl.cn

Go:   encoding/gob
来源：http://iql.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://pyc.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xfj.wangshuangyany.cn

================================================================================
来源：http://aqq.yj202588.top

L. 网络请求
来源：http://znd.sweek.top

================================================================================
来源：http://han.shangyingyoupin.top

[L01] 发送 GET 请求
来源：http://wst.fehbvm.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nac.andypj.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uve.cqqwz.cn

JS:   await fetch(url)
来源：http://msa.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://ebk.ctjpmb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zfu.jlsjyb.cn

Go:   resp, err := http.Get(url)
来源：http://aio.shuidangran.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tpt.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hng.hywenlv.cn

[L02] 发送 POST JSON
来源：http://xtq.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dav.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ltt.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iwg.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cgp.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vkk.jianghu66.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://urh.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bwe.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nwc.smart0.xyz

[L03] 设置自定义请求头
来源：http://xhe.mhx1999.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ohp.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rer.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zqt.52xcode.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rgu.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ver.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lwr.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jun.nanxuanxn.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://skg.9152youxi.cn

[L04] 设置超时
来源：http://gkr.yanxiufei.cn

Py:   requests.get(url, timeout=5)
来源：http://dui.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jbc.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yxu.gogol.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://unz.wangshuangyany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://coa.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fyv.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://imz.ehwqpu.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://szg.fzhhl.top

[L05] 上传文件（multipart）
来源：http://eon.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://knn.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sjw.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tzh.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dit.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://alr.svipenyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yhh.aibaodan.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://req.shuidangran.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hru.fehbvm.com

[L06] 解析响应为 JSON
来源：http://fow.fanxiaobao.xyz


<!-- 参考信息 -->