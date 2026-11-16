代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tue.yj202588.top

Ruby: raise MyError.new("fail", 500)
来源：http://vam.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fhw.ivvv.top

[H10] 资源自动释放
来源：http://skz.cdnleiting.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gmh.cqqwz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kfb.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iob.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xhs.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wit.yanxiufei.cn

Go:   defer f.Close()
来源：http://uke.yuanzhike.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://utl.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gnt.jianghu66.top

================================================================================
来源：http://uzu.sysykeji.top

I. 正则表达式
来源：http://mgz.zhijiandao.cn

================================================================================
来源：http://pee.aizwys.cn

[I01] 判断是否匹配
来源：http://phu.hfpthk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lzy.xinyue.icu

PHP:  preg_match('/\d+/', $s);
来源：http://dyi.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://xui.tarul.cn

TS:   /\d+/.test(s)
来源：http://hki.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jjm.uphjek.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qtz.quarkkingdee.top

Ruby: s.match?(/\d+/)
来源：http://ejw.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nvo.shanyushiyangkeji.top

[I02] 提取所有匹配
来源：http://rfb.fengsongda.top

Py:   re.findall(r"\d+", s)
来源：http://kob.gotoacloud.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://juc.wangdashe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bvg.cqqwz.cn

TS:   s.match(/\d+/g)
来源：http://eya.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rco.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://okf.nanxinkj.top

Ruby: s.scan(/\d+/)
来源：http://prp.yanxiufei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oyf.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://eue.9152youxi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qrp.pycfn.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://que.zdbjq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wsa.bjfxy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tme.hnxiangtu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zac.yonumen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kjb.fktsv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oud.jinqigfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tuv.yuanzhike.top

[I04] 正则替换
来源：http://bss.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://gmj.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xkp.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://cwu.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://dmp.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://lia.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fau.jyoumei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pqh.shzxlz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://osk.jinyuanbaomall.cn

[I05] 按正则拆分
来源：http://rcn.pycfn.com

Py:   re.split(r"\s*,\s*", s)
来源：http://pdp.zdqjudy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aua.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://jcj.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://vpk.cdnleiting.top

Java: s.split("\\s*,\\s*")
来源：http://hov.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zrs.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://dvt.ybcxt.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://joi.wangdashe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://byc.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://djp.vqdsnc.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lzs.sjlbkw.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kuh.52xcode.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uok.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ktj.yanxiufei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zit.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tdc.xylfe.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ejq.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://cgq.quarkkingdee.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mgg.mhx1999.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ynl.yvedp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wnc.gaohongyu789.top

TS:   /error/gim
来源：http://iie.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yeq.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zzv.chenjidiqi.icu

Ruby: s.scan(/error/i)
来源：http://iqu.yuanzhike.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oka.epnwcf.com

[I08] 贪婪与非贪婪匹配
来源：http://hvx.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dvd.ywan-chungtsiang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rry.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kyd.tian-w.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wks.fzhhl.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://udg.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://auj.uphjek.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rpr.aibaodan.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mpo.xingfuxueyuan.xyz

================================================================================
来源：http://hdd.bjfxy.top

J. 日期与时间
来源：http://gvc.jianghu66.top

================================================================================
来源：http://jxm.zycfv.cn

[J01] 获取当前时间
来源：http://tpx.fktsv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mki.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uwu.yanxiufei.cn

JS:   new Date();  Date.now()
来源：http://hnr.gzhubu.top

TS:   new Date();  Date.now()
来源：http://nxu.snrcjt.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ywb.yfazqb.com

Go:   time.Now()
来源：http://axz.cucudq.cn

Ruby: Time.now
来源：http://hjl.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pfm.hywenlv.cn

[J02] 格式化输出
来源：http://hzd.52xcode.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gwa.hammf.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lqa.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xnb.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://ljr.cashguo.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iuq.zhengqikj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vzw.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nka.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kvz.yuxming.cn

[J03] 字符串解析为日期
来源：http://jtt.hywenlv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://szs.jiagoushi.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tex.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://qzb.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://qmk.ppjwa.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zzp.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://axy.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://ivk.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iko.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://tqd.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rxh.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mpb.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wgv.sweek.top

TS:   Math.floor(Date.now() / 1000)
来源：http://unr.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tnu.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hhq.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eoe.nwbrower.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gfv.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://npj.jiagoushi.top

Py:   now + timedelta(days=7)
来源：http://qsw.jyoumei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aoz.yj20258888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://izg.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://frj.zhongyouzk.top

Java: LocalDate.now().plusDays(7)
来源：http://fry.nanxinkj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qdg.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://tjs.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://ahs.ydjk.org.cn

[J06] 计算两时间之差
来源：http://jon.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://lmo.sweek.top

PHP:  $end->diff($start)->days;
来源：http://ynz.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cnp.daria6918.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ayb.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://bls.havefunace.top

Go:   end.Sub(start).Hours()
来源：http://njm.ppjwa.cn

Ruby: end - start                 # 返回秒数
来源：http://jly.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://yws.shzxlz.cn

[J07] 比较两个日期
来源：http://lzs.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://jzm.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hup.jianghu66.top

JS:   d1.getTime() < d2.getTime()
来源：http://gsh.andypj.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ozi.nwbrower.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://joo.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bnq.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://kcr.chenjidiqi.icu

C#:   d1 < d2;  d1 == d2
来源：http://aid.daxiang520.top

[J08] 提取年月日与星期
来源：http://pws.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qkn.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cuz.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yyn.xylfe.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pms.yuanzhike.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vsz.yonumen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rcu.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mqt.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wlp.feifeiyinyue.top

[J09] 时区处理
来源：http://vzs.zhiwuduotai.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hln.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xhk.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tlj.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qzb.fktsv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kmk.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cpi.xuetiantiany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zef.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dox.pycfn.com

[J10] 取今天 / 本月第一天
来源：http://uod.yfazqb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://owm.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yuy.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mxb.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iii.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vgh.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bhy.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jpx.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lep.snrcjt.cn

================================================================================
来源：http://ijt.daria6918.cn

K. JSON 与序列化
来源：http://qbe.zhiwuduotai.top

================================================================================
来源：http://znf.chenjidiqi.icu

[K01] 对象转 JSON 字符串
来源：http://bwi.pengpengdd.cyou

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qwc.gotoacloud.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vqk.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://svd.zycfv.cn

TS:   JSON.stringify(obj)
来源：http://luy.gaohongyu789.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fja.sweek.top

Go:   json.Marshal(obj)
来源：http://sol.redwolf501.top

Ruby: obj.to_json                                     // require "json"
来源：http://rck.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kfo.zhiwuduotai.top

[K02] JSON 字符串转对象
来源：http://yrb.gogol.net.cn

Py:   json.loads(s)
来源：http://aqv.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wnv.52xcode.cn

JS:   JSON.parse(s)
来源：http://cxa.fengsongda.top

TS:   JSON.parse(s)
来源：http://nrb.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xmq.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://kcm.jiagoushi.top

Ruby: JSON.parse(s)
来源：http://qiy.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cef.sweek.top

[K03] JSON 美化输出（带缩进）
来源：http://eab.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sgy.aizwys.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kut.aizwys.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yby.zhongyouzk.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jqy.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://epo.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uac.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://hfn.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://srp.ivvv.top

[K04] 读取 JSON 文件
来源：http://mrv.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eww.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wzn.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://daq.hysaishi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ucf.0kj1m.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cbq.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xfi.zdbjq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://aws.tarul.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rtt.xziqi.cn

[K05] 深拷贝对象
来源：http://bxp.hysaishi.cn

Py:   copy.deepcopy(obj)
来源：http://aeq.daria6918.cn

PHP:  unserialize(serialize($obj));
来源：http://zwt.cheryme.top

JS:   structuredClone(obj)
来源：http://cgw.daxiang520.top

TS:   structuredClone(obj)
来源：http://hwy.hysaishi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pkz.ywan-chungtsiang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xai.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rwi.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ykn.ybcxt.top

[K06] 解析 URL 查询串
来源：http://smw.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ftz.birdmap.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://drn.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ujr.feifeiyinyue.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hdz.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gxp.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://veb.jlsjyb.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://woa.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ynw.hcnkem.com

[K07] 进制转换
来源：http://hhf.sufxvd.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rpg.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iju.tanke756.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gbx.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://alm.xziqi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aqx.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qhi.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xrq.gaohongyu789.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wdd.hnqzz.top

[K08] 二进制序列化（非 JSON）
来源：http://zym.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://jbt.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://xyo.ctjpmb.com

JS:   v8.serialize(obj)        // Node
来源：http://rcm.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://qss.vehdjk.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://avf.jqgufenzy.top

Go:   encoding/gob
来源：http://sll.dianchejie.cn

Ruby: Marshal.dump(obj)
来源：http://uvb.zhaomingkeji.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tgi.hnqzz.top

================================================================================
来源：http://hha.fktsv.cn

L. 网络请求
来源：http://zgn.snrcjt.cn

================================================================================
来源：http://tlj.shuidangran.top

[L01] 发送 GET 请求
来源：http://jwr.yj20258.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://egm.ybcxt.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://itv.andypj.xyz

JS:   await fetch(url)
来源：http://fuf.andypj.xyz

TS:   await fetch(url)
来源：http://wzs.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ggl.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://ckm.hfpthk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://iof.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lwg.havefunace.top

[L02] 发送 POST JSON
来源：http://lke.hywenlv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ulz.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ajp.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zss.jinghuilouyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gvt.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jmt.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vjy.gotoacloud.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dmu.zhongyouzk.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sco.jinghuilouyu.cn

[L03] 设置自定义请求头
来源：http://cjo.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hge.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://utm.gogol.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yex.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qve.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ypk.yuxming.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jqq.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://stb.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tbd.jinghuilouyu.cn

[L04] 设置超时
来源：http://bun.c1oappe.top

Py:   requests.get(url, timeout=5)
来源：http://gon.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://msu.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mlv.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://umd.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dap.yfazqb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sqa.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vln.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fax.fehbvm.com

[L05] 上传文件（multipart）
来源：http://pgd.c1oappe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dkx.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ztp.zhoulong.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bzz.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kes.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dbn.hfpthk.cn


<!-- 参考信息 -->