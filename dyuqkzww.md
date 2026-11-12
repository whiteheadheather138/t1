代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://yjd.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ktg.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iqq.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jks.chenjidiqi.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eds.tarul.cn

Go:   defer f.Close()
来源：http://pdk.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tlq.zhaomingkeji.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ckm.jinyuanbaomall.cn

================================================================================
来源：http://ato.yj20258888.top

I. 正则表达式
来源：http://zdp.316326.xyz

================================================================================
来源：http://jnc.kuanghao11.cn

[I01] 判断是否匹配
来源：http://cnk.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hlr.jianghu66.top

PHP:  preg_match('/\d+/', $s);
来源：http://yet.fengsongda.top

JS:   /\d+/.test(s)
来源：http://emi.yonumen.top

TS:   /\d+/.test(s)
来源：http://qmg.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oyg.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wwi.aizwys.cn

Ruby: s.match?(/\d+/)
来源：http://ygo.shuidangran.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zph.jinghuilouyu.cn

[I02] 提取所有匹配
来源：http://ltz.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://ylu.hcnkem.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://spp.zhongyouzk.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vbc.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://tqh.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bed.sxryk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://arj.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://dys.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yji.bbcook.cn

[I03] 提取捕获分组
来源：http://uqd.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ait.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ohg.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qct.fehbvm.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zgl.zhongyouzk.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://szt.ywan-chungtsiang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fst.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hjz.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ria.shangyingyoupin.top

[I04] 正则替换
来源：http://dnm.hfpthk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://aoe.ppjwa.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xxt.zhongyouzk.top

JS:   s.replace(/\d+/g, "#")
来源：http://jtn.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yvc.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bio.52xcode.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tib.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vyx.nanxuanxn.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://asv.birdmap.top

[I05] 按正则拆分
来源：http://mqv.jianghu66.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jfw.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eyt.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://vxp.ywan-chungtsiang.top

TS:   s.split(/\s*,\s*/)
来源：http://qzq.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://jej.kuanghao11.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kqy.ydzc1.top

Ruby: s.split(/\s*,\s*/)
来源：http://bcp.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://urw.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nxo.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bmj.vehdjk.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eak.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wbi.andypj.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dgh.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bpq.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zjc.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lfc.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://foc.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://njs.xuetiantiany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ruj.cdnleiting.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zoy.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kvd.tanke756.top

TS:   /error/gim
来源：http://wbn.9152youxi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://htl.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yve.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://lbr.aibaodan.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ilf.cheryme.top

[I08] 贪婪与非贪婪匹配
来源：http://uka.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ncr.shuidangran.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dly.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lmt.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nci.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jkc.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iku.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cqu.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jmu.nwbrower.top

================================================================================
来源：http://gjq.0kj1m.cn

J. 日期与时间
来源：http://itf.shanyushiyangkeji.top

================================================================================
来源：http://hdv.hnqzz.top

[J01] 获取当前时间
来源：http://kyd.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ekk.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ytj.jianghu66.top

JS:   new Date();  Date.now()
来源：http://roc.ywan-chungtsiang.top

TS:   new Date();  Date.now()
来源：http://wcs.ywan-chungtsiang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://glz.shzxlz.cn

Go:   time.Now()
来源：http://eoj.shanyushiyangkeji.top

Ruby: Time.now
来源：http://nzn.tianlin.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wgb.jyoumei.cn

[J02] 格式化输出
来源：http://ahv.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uma.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pki.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xkt.nanxuanxn.top

TS:   d.toISOString()
来源：http://nyj.zhoulong.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://whx.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cmo.uphjek.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jvj.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tvf.smart0.xyz

[J03] 字符串解析为日期
来源：http://gcx.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pzq.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xwc.ppjwa.cn

JS:   new Date("2024-01-02")
来源：http://ujn.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://yas.yj202588.top

Java: LocalDate.parse("2024-01-02")
来源：http://zaj.yanxiufei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fjz.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://bsk.ywan-chungtsiang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vbc.fengsongda.top

[J04] 时间戳与日期互转
来源：http://pvx.shzxlz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vmg.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vmc.vqdsnc.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ven.fzhhl.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vje.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vyt.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lpw.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nev.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oug.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://opq.ydzc1.top

Py:   now + timedelta(days=7)
来源：http://xbe.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://hvg.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jgs.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rtd.ppjwa.cn

Java: LocalDate.now().plusDays(7)
来源：http://qnh.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zet.ywan-chungtsiang.top

Ruby: Time.now + 7 * 86400
来源：http://vcj.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://qxf.daxiang520.top

[J06] 计算两时间之差
来源：http://zmw.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://skv.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://ghu.aizwys.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uvn.fzhhl.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nib.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://bha.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://djq.fehbvm.com

Ruby: end - start                 # 返回秒数
来源：http://zps.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://pka.wangdashe.top

[J07] 比较两个日期
来源：http://hfa.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://uac.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kfi.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gem.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://pio.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hqr.feifeiyinyue.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hze.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://oyj.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://rur.yj20258.top

[J08] 提取年月日与星期
来源：http://bns.hywenlv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ztf.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ent.yongpay.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nbr.cashguo.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gsz.zdbjq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dbi.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://shw.shzxlz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sbo.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fvs.shzxlz.cn

[J09] 时区处理
来源：http://qws.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bfp.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wdr.shanyushiyangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pwt.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ska.sxryk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wbi.uphjek.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mtz.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://vmy.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lfu.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://bwv.tian-w.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ejv.vehdjk.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sns.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ywv.fehbvm.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pho.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lnn.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qvl.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yah.daxiang520.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://grx.yuxming.cn

================================================================================
来源：http://mqi.zhengqikj.top

K. JSON 与序列化
来源：http://yxw.sxryk.cn

================================================================================
来源：http://wnb.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://iop.pengpengdd.cyou

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bmy.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uus.yueranfly.top

JS:   JSON.stringify(obj)
来源：http://ajm.jqgfzy.top

TS:   JSON.stringify(obj)
来源：http://hvp.gaohongyu789.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ive.daria6918.cn

Go:   json.Marshal(obj)
来源：http://uaz.haohaochexian.top

Ruby: obj.to_json                                     // require "json"
来源：http://lfo.xylfe.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ceg.shuidangran.top

[K02] JSON 字符串转对象
来源：http://wjx.feifeiyinyue.top

Py:   json.loads(s)
来源：http://sjm.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://olx.zhixingplan.top

JS:   JSON.parse(s)
来源：http://vym.xziqi.cn

TS:   JSON.parse(s)
来源：http://civ.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zwr.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://vdu.sjlbkw.cn

Ruby: JSON.parse(s)
来源：http://ylj.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nyj.zhiwuduotai.top

[K03] JSON 美化输出（带缩进）
来源：http://uea.svipenyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://adc.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pwn.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://aet.quarkkingdee.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ajn.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qvn.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sjl.wangshuangyany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lcf.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ysg.hesvh.cn

[K04] 读取 JSON 文件
来源：http://rup.hysaishi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uvl.svipenyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lxk.hysaishi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lkf.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://boe.mhx1999.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lwj.xziqi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ymn.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xpe.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ydy.gotoacloud.top

[K05] 深拷贝对象
来源：http://eno.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://die.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://ptb.ehwqpu.com

JS:   structuredClone(obj)
来源：http://wwm.yuxming.cn

TS:   structuredClone(obj)
来源：http://dul.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tbn.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://slf.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://okx.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fdf.jqgfzy.top

[K06] 解析 URL 查询串
来源：http://aee.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fxi.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gxd.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mns.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://agy.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sty.zdbjq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vvs.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vqo.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://loi.jqgfzy.top

[K07] 进制转换
来源：http://sgq.andypj.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://scd.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pcv.tianlin.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kzg.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jbd.0kj1m.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uqt.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yrh.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://txd.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vxw.gzhubu.top

[K08] 二进制序列化（非 JSON）
来源：http://btj.hywenlv.cn

Py:   pickle.dumps(obj)
来源：http://rrr.jinqigufen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gev.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://jqm.jianghu66.top

TS:   v8.serialize(obj)        // Node
来源：http://opf.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rhw.yfazqb.com

Go:   encoding/gob
来源：http://ejp.zhongyouzk.top

Ruby: Marshal.dump(obj)
来源：http://cwt.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uhv.ehwqpu.com

================================================================================
来源：http://qsn.yvedp.cn

L. 网络请求
来源：http://dnf.hywenlv.cn

================================================================================
来源：http://mos.chenzaomai.com

[L01] 发送 GET 请求
来源：http://stq.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cyz.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://stf.cashguo.top

JS:   await fetch(url)
来源：http://gso.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://qri.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tcg.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://wzj.yuxming.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yvj.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kdi.yanxiufei.cn

[L02] 发送 POST JSON
来源：http://mda.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://aty.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hhj.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eim.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qgp.cashguo.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wyo.sxryk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rqd.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jfd.yvedp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hnp.gzhubu.top

[L03] 设置自定义请求头
来源：http://fww.havefunace.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ywl.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://piy.nanxuanxn.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hzj.yfazqb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vud.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pcs.daxiang520.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lak.yueranfly.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xwd.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pvr.sysykeji.top

[L04] 设置超时
来源：http://yth.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://tdr.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wti.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qnh.zhixingplan.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zol.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dby.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tke.vqdsnc.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kgr.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wib.pycfn.com

[L05] 上传文件（multipart）
来源：http://chi.daria6918.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ehu.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dpp.chenjidiqi.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pes.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iuv.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://whn.shuidangran.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yts.ehwqpu.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kfb.yuxming.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ctw.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://man.ivvv.top


<!-- 参考信息 -->